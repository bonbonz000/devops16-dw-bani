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

     ![2](https://user-images.githubusercontent.com/91004163/236704040-b7632f26-b4ce-46d3-9f15-303c8fa7fdb3.PNG)

     ![1](https://user-images.githubusercontent.com/91004163/236704017-23c53ae2-0cf7-4300-b8c4-13616fb07023.PNG)

     
     
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
