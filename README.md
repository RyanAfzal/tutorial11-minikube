# Tutorial-11
---
#### Nama: Ryandhika Al Afzal
#### NPM: 2206081502
#### Kelas: Adpro A
---
### Reflection (1) Hello Minikube
1. **Compare the application logs before and after you exposed it as a Service.** <br>
![image](https://github.com/RyanAfzal/tutorial11-minikube/assets/137851158/53616e3e-d7ac-49d6-8e89-958605c50372)<br>

Ya ada perbedaan, sebelum service diexposed, tidak ada log yang ditampilkan ketika ada browser yang dibuka. Setelah service diexposed, service dapat menerima request sehingga log akan mencatat request yang telah dibuat, contoh request tersebut dapat dilihat pada gambar di atas. 

2. **Notice that there are two versions of `kubectl get` invocation during this tutorial section. The first does not have any option, while the latter has `-n` option with value set to `kube-system`. What is the purpose of the `-n` option and why did the output not list the pods/services that you explicitly created?** <br>
Perbedaan antara kedua sintaks tersebut adalah dengan menggunakan <code>-n</code>. <code>-n</code> adalah singkatan dari namespace. -n option diperlukan jika ada banyak service berbeda yang memiliki nama yang sama dan tersebar di berbagai namespace. Dengan menggunakan -n option kita dapat mengarahkan get ke namespace yang kita berikan setelah query -n.