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
     
![dns record](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/9cc44b57-932c-4ad9-a840-8fdec36c45e4)


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
     
Ansible Aplikasi wayshub

![image](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/d8afa3ac-d1d5-47f5-ac97-b66c586026d9)

     
aplikasi wayshub running
     
![ansible deploy 4](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/d1e88583-8f3d-4185-b1e8-fc030d7d507c)
     
     
playbook Docker
  
![image](https://user-images.githubusercontent.com/91004163/236728240-942fdd74-a4c2-403c-8fe7-93b818449179.png)

     
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

 Setup node-exporter, prometheus dan Grafana menggunakan docker
     
 ![9](https://user-images.githubusercontent.com/91004163/236971912-f770f7d6-02d5-43f9-9fb1-fcce455d1380.PNG)
     
 install node-exporter di appserver & gateway
     
![node exp 1](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/216825f7-ac88-488e-b88f-021da2c1cec8)
     
![node exp 2](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/78eb38e1-36cb-4fb9-b498-2f8cd8728fb0)
     
![image](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/36fb76a2-0834-41b7-a0ff-8d39d0b8f9bc)
     
Dashboard untuk monitor resource server (CPU, RAM & Disk Usage)

![grafana 1](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/c4c4104c-be69-4c0f-b401-46bbd0a8f1f3)
     
     
 Alerting Telegram
     
![bot tele1](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/03b63aa5-2ce8-4ddc-859a-ac299abb7677)

![bot tele2](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/10a797b1-816d-47cc-a2c2-0ad691de74e2)

![bot tele3](https://github.com/bonbonz000/devops16-dw-bani/assets/91004163/8ef172bb-d0bb-4afd-bc9f-e79d0cdf1e60)


     


