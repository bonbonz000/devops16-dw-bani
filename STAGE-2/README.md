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

APPSERVER idcloudhost

![appserv](https://user-images.githubusercontent.com/91004163/230774957-b20a4de3-20ca-42e8-99de-9d2be091dbe4.png)

Gateway server idcloudhost

![gatewayserv](https://user-images.githubusercontent.com/91004163/230774965-e989693a-3877-498d-8fa7-ce53d5ab2e5c.png)

domain be and fe

![domain be dan fe](https://user-images.githubusercontent.com/91004163/230775288-03c2e12c-6b08-4ee1-83fc-3e5c99756fd1.png)



1.NODE VERSI 14 

![node v 14](https://user-images.githubusercontent.com/91004163/230774229-83cb9c05-8a7d-44cb-99a4-ec3246873442.png)

2.repo clone FE dan BE 

![clonned wayshub](https://user-images.githubusercontent.com/91004163/230774253-b8b908ea-5fa2-42ed-a3fd-2482e0ac3a58.png)


3.mysql database install


![mysql_secure_installation](https://user-images.githubusercontent.com/91004163/230774296-235710f0-4b34-4ea0-b3cf-2fa72514fac4.png)

db wayshub

![db_wayshub](https://user-images.githubusercontent.com/91004163/230774481-d7049afd-bfcd-450f-883e-2f392864326b.png)

frontend BaseURL configuration in : src/config/api.js

![baseurl config Frontend - appserver](https://user-images.githubusercontent.com/91004163/230782987-543e1120-f941-4516-a763-5dbdc140ae28.png)



backend database configuration in : config/config.json


![database config backend - appserver](https://user-images.githubusercontent.com/91004163/230776033-818a88a2-0cfe-4696-a54c-fdfd9e5dd738.png)

install npm sequelize :

![1](https://user-images.githubusercontent.com/91004163/230799544-0b9b3e7a-8127-418a-87bd-ceb309d154e7.png)


sequelize db:create

![2](https://user-images.githubusercontent.com/91004163/230799548-44873b1f-8a3a-4d26-82be-c5eb5182cd42.png)


sequelize db:migrate

![3](https://user-images.githubusercontent.com/91004163/230799555-7272702d-4fc3-4617-9dc6-8b9a426a90d5.png)

show databases

![4](https://user-images.githubusercontent.com/91004163/230799566-3fb7f7c1-eced-41a6-b8e9-658c615e4474.png)



Deploy in PM2 with ecosystem simple

FE config

![ecosystem frontend config](https://user-images.githubusercontent.com/91004163/230774370-4d705823-bfd4-4853-b359-9c4ddaa036fc.png)


BE config

![backend ecosystem config](https://user-images.githubusercontent.com/91004163/230774376-a1b80bfa-94cc-4b7f-b361-96425e63f658.png)

run with pm2

![run with pm2 ecosystem simple](https://user-images.githubusercontent.com/91004163/230774335-5ae8fbc1-ecb7-457f-956c-767f8592c179.png)



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

nginx installation

![gateway server - nginx install](https://user-images.githubusercontent.com/91004163/230775130-42673df0-bc55-4df1-ad2d-5cf8fc209231.png)

reverse proxy config in : /etx/nginx/dumbways/

![rproxy config](https://user-images.githubusercontent.com/91004163/230775164-6e16e140-54ec-423a-901e-fd6962a549de.png)


include in nginx.conf

![nginx include in nginx conf](https://user-images.githubusercontent.com/91004163/230776340-05d4641a-2353-4b53-8104-d136455f61da.png)

wayshub frontend from domain name

![wayshub FE from domain](https://user-images.githubusercontent.com/91004163/230797829-277921ff-b5c0-4123-a6ae-58af192101dc.png)


CHALLENGE

TASK :

Instructions :
[Certbot Instructions for Ubuntu 20.04 with Nginx](https://certbot.eff.org/instructions?ws=nginx&os=ubuntufocal)

Tasks :
1. Pastikan domain sudah mendapatkan https (secure)
2. Ikuti instruksi dari certbot

Answer :

1.

2.
snapd install

![snapd install](https://user-images.githubusercontent.com/91004163/230786763-95b1b6e6-a44a-4ffa-8c6c-a07dfd15d585.png)

certbot install

![install certbot](https://user-images.githubusercontent.com/91004163/230786764-a7029b39-7193-4e25-86cf-c8f0ff732aa0.png)

create shortcut link

![create link certbot](https://user-images.githubusercontent.com/91004163/230786772-14d4b32d-2f71-4d1d-8d2d-616be0d1375c.png)

install certbot 

![generate certbot](https://user-images.githubusercontent.com/91004163/230786779-79a7c87b-65ee-4239-96dc-29934799d9c6.png)


