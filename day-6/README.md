Question :
1. Buat 1 VM tambahan untuk nginx saja (Ini opsional ya, tidak wajib)
2. Jalankan aplikasi Dumbflix menggunakan PM2
3. Buatlah reverse proxy dengan directory /etc/nginx/dumbways
4. Dengan nginx, pastikan dumbflix bisa diakses ke domain yang diinginkan

Answer :

1.


2.dumbflix di dalam pm2

![1](https://user-images.githubusercontent.com/91004163/227361737-a3d1ffe1-2aee-406f-ab0e-ac1bbe184a9a.png)

3.reverse proxy

create and setup proxy config file

![2](https://user-images.githubusercontent.com/91004163/227361871-6c5b7824-3b51-4601-82f2-72116b1cb141.png)

setup include nginx conf to read the folder contain reverse proxy

![4](https://user-images.githubusercontent.com/91004163/227362003-4eef35d0-1ded-454a-8757-7721ccaf4efb.png)

nginx test , restart and check status

![5](https://user-images.githubusercontent.com/91004163/227362382-3f148739-f589-4469-9af5-e88d0ff7cfe7.png)


add domain di host windows


![3](https://user-images.githubusercontent.com/91004163/227361950-46d59699-a405-4e9a-861f-615aa4782080.png)


custom domain accessable ceksoundmase.xyz

![6](https://user-images.githubusercontent.com/91004163/227362577-44ad8167-93d5-4a11-b3ab-6db4d5b1075f.png)



