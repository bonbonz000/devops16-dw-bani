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

