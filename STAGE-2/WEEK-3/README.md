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

Tasks :
- Buatlah script Terraform untuk membuat 3 server sesuai dengan kebutuhan
- Pastikan semua server mendapatkan Floating IP (IP Public)
- OS yang digunakan : Ubuntu 20.04


Answer:

     
     
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
     
     
     
