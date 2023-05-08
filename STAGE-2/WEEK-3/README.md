DOMAIN

Task:

Gunakan domain dengan SSL :
     - Node-exporter
node-exporter.<nama>.studentdumbways.my.id
        -  Prometheus
prom.<nama>.studentdumbways.my.id
         -  Grafana
dashboard.<nama>.studentdumbways.my.id
          -  App frontend
<nama>.studentdumbways.my.id

Answer:

TERRAFORM

Task:

Buat 3 VM dengan *Terraform* di IDCloudHost dengan spesifikasi sebagai berikut :
   - Appserver : 1 CPU, 1 GB RAM
   - Gateway : 1 CPU, 1 GB RAM
   - Monitoring : 2 CPU, 2GB RAM
    Storage : 20 GB
     
- Buatlah script Terraform untuk membuat 3 server sesuai dengan kebutuhan
- Pastikan semua server mendapatkan Floating IP (IP Public)
- OS yang digunakan : Ubuntu 20.04


Answer:

Terraform config
     
![2](https://user-images.githubusercontent.com/91004163/236704086-196152eb-a091-4642-a5d5-e19f252ddfb3.PNG)


 Server created
     
![1](https://user-images.githubusercontent.com/91004163/236704084-e8e70950-48e6-4e1e-a891-4ba88764f234.PNG)

     
     
Ansible
     
Tasks :
- Setup inventory dan ansible menggunakan SSH key
- Buatlah Ansible Playbook :

[appserver]
- Instalasi docker dan menjalankan aplikasi frontend week 2
- User baru (gunakan user barunya untuk semua konfigurasi ansible)

[gateway]
- Instalasi nginx
- konfigurasi nginx dan reverse proxy sampai bisa menggunakan domain
- User baru (gunakan user barunya untuk semua konfigurasi ansible)
     
Answer :

Docker installation config

![image](https://user-images.githubusercontent.com/91004163/236724701-6372f51e-d292-480c-9b10-76e656951725.png)
     
 Setup inventory dan ansible dengan SSH key
     
![3](https://user-images.githubusercontent.com/91004163/236711834-538efe11-38f8-4682-809f-6bcf4aae2724.PNG)

 Playbook gateway
     
![4](https://user-images.githubusercontent.com/91004163/236712009-a1057e23-0f32-4cbd-9a20-33e045d4e4a9.PNG)
     
 run nginx

![5](https://user-images.githubusercontent.com/91004163/236712542-573d262b-a3ff-40a6-a322-5efd8b57050b.PNG)
     

access nginx

![6](https://user-images.githubusercontent.com/91004163/236712550-ad5725fd-89f8-4c74-9861-cd2187588f33.PNG)
     
     
PROMETHEUS + GRAFANA
     
Docker Images :
[node-exporter](https://hub.docker.com/r/prom/node-exporter)
[Prometheus](https://hub.docker.com/r/prom/prometheus)
[Grafana Dashboard](https://hub.docker.com/r/grafana/grafana)


Tasks :
     
- Setup node-exporter, prometheus dan Grafana menggunakan docker
- install node-exporter di appserver & gateway
- Dengan Grafana, buatlah :
    -  Dashboard untuk monitor resource server (CPU, RAM & Disk Usage)
    -  Buat alerting dengan Contact Point pilihan kalian (discord, telegram, slack dkk)
    -  Untuk alert :
         - CPU Usage over 20%
         - RAM Usage over 75%

     
 Answer:
