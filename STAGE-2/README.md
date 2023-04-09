PART 1

TASK:


Buat 2 VM di IDCloudHost dengan spesifikasi sebagai berikut :
   - Appserver : 1 CPU, 2 GB RAM
   - Gateway : 1 CPU, 1 GB RAM
    Storage : 20 GB

Repository :
[Wayshub Frontend](https://github.com/dumbwaysdev/wayshub-frontend)
[Wayshub Backend](https://github.com/dumbwaysdev/wayshub-backend)


Tasks :
[ Appserver ]

    - Gunakan nodejs versi 14.x
    - Clone repository Wayshub frontend & backend lalu deploy aplikasinya menggunakan PM2
    - Install dan konfigurasi database MySQL (mysql_secure_installation)
    - Di wayshub-frontend, rubah isi BaseURL file src/config/api.js menggunakan domain yang sudah disediakan (api.<nama>.studentdumbways.my.id)
    - Di wayshub-backend, rubah isi konfigurasi database MySQL di config/config.json sesuai dengan user pass kalian, dengan nama database "db-wayshub"


Answer :

1.NODE VERSI 14 

![node v 14](https://user-images.githubusercontent.com/91004163/230774229-83cb9c05-8a7d-44cb-99a4-ec3246873442.png)

2.repo clone FE dan BE 

![clonned wayshub](https://user-images.githubusercontent.com/91004163/230774253-b8b908ea-5fa2-42ed-a3fd-2482e0ac3a58.png)


Deploy in PM2 with ecosystem simple

FE config

![ecosystem frontend config](https://user-images.githubusercontent.com/91004163/230774370-4d705823-bfd4-4853-b359-9c4ddaa036fc.png)


BE config

![backend ecosystem config](https://user-images.githubusercontent.com/91004163/230774376-a1b80bfa-94cc-4b7f-b361-96425e63f658.png)

run with pm2

![run with pm2 ecosystem simple](https://user-images.githubusercontent.com/91004163/230774335-5ae8fbc1-ecb7-457f-956c-767f8592c179.png)



3.mysql database install


![mysql_secure_installation](https://user-images.githubusercontent.com/91004163/230774296-235710f0-4b34-4ea0-b3cf-2fa72514fac4.png)


PART 2

TASK :


Buat 2 VM di IDCloudHost dengan spesifikasi sebagai berikut :
   - Appserver : 1 CPU, 2 GB RAM
   - Gateway : 1 CPU, 1 GB RAM
    Storage : 20 GB

Tasks :
[ Gateway ]

    - Installasi nginx di server gateway
    - Buat konfigurasi reverse proxy di dalam directory : /etc/nginx/dumbways
    - Gunakan domain :
       - <nama>.studentdumbways.my.id (front-end)
       - api.<nama>.studentdumbways.my.id (back-end)
        note : <nama> diganti sesuai dengan nama kalian.


Answer:



CHALLENGE

TASK :

Instructions :
[Certbot Instructions for Ubuntu 20.04 with Nginx](https://certbot.eff.org/instructions?ws=nginx&os=ubuntufocal)

Tasks :
1. Pastikan domain sudah mendapatkan https (secure)
2. Ikuti instruksi dari certbot

Answer :

