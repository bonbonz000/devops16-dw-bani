Question :

PART 1.
1. Jelaskan apa itu Bourne-Again Shell (BASH)!
2. Instalasi NGINX dan pastikan bisa di akses melalui lokal kalian.
3. Jalankan 5 command linux shell beserta fungsinya!

Answer :

1.Bourne-Again Shell (BASH) adalah command languange interpreter untuk berinteraksi dengan sistem operasi menggunakan perintah-perintah spesifik.
Disebut shell karena shell menyebunyikan kernel dari kerumitan yang terjadi di dalamnya, sehingga memungkinkan pengguna untuk fokus pada command
spesifik untuk menjalankan suatu fungsi.

2.

3.![1](https://user-images.githubusercontent.com/91004163/224894288-018cdac6-a8bd-4031-a31b-545c27d56d63.png)

![2](https://user-images.githubusercontent.com/91004163/224894304-9432ad5b-101a-4494-8f41-16eeab708c35.png)

![3](https://user-images.githubusercontent.com/91004163/224894312-8e8e4c12-6a91-488f-9004-0deebd00f956.png)

Keterangan:

1.pwd(print working directory) - untuk mengecek current directory
2.whoami -  untuk mengecek user yang sedang digunakan
3.ifocnfig -  untuk mengecek detail dari network di mesin
4.echo - untuk menampilkan konten dari  file, bis di gabungkan dengan redirect+add >> untuk menambahkan ke file yang diinginkan.
5.less -  untuk membuka file spesifik ditambah dengan fungsi navigasi

PART 2.

1. Jelaskan perbedaan antara IP Public dan IP Private!

IP PUBLIK :
  ip (internet protocol) publik merupakan alamat unik dari device di dalam network yang dapat di kenali di internet dan memiliki segmentasi IP yang berbeda
  dari ip private dan tidak dapat sembarangan diubah oleh client dikarenakan sudah diatur oleh ISP. Terdapat dua jenis IP publik yaitu : static dan dynamic.
  
IP PRIVATE:
  ip (internet protocol) private merupakan alamat unik dari device di dalam network yang tidak dapat dikenali di internet, melainkan hanya di jaringan lokal saja.
  IP private memiliki segmentasi IP berbeda dari IP publik. Terdapat range kelas subnet yang dapat diterapkan di IP Private.

3. Jelaskan perbedaan antara Client-to-Server dan Peer-to-peer!

  Client-to-Server :
    Client-to-Server memiliki server yang tersentral, sehingga client akan fokus untuk mengakses satu server saja.
    Kekurangan :  1.layanan tidak akan tersedia jika server sentral mati
                  2.cenderung lebih mahal dalam penerapannya
                  3.memerlukan hardware high-end untuk servernya
                  
    kelebihan :   1.kapabilitas backup akan lebih mudah karena hanya satu server
                  2.akan lebih mudah diamankan dari serangan cyber karna hanya perlu fokus kepada satu server
                  3.akses pada jaringan akan lebih cepat
                  
  Peer-to-Peer :
    Peer-to-Peer memiliki server yang tidak tersentral, dalam topologi ini client bisa bertindak sebagai server dan sebaliknya.
    kekurangan :  1.lebih rentan terkena serangan cyber ke seluruh device di jaringan jika konfigurasi kemanan tidak optimal di masing-masing device.
                  2.backup harus di lakukan di setiap device di dalam jaringan
                  
    kelebihan :   1.layanan akan tetap tersedia jika salah satu server mati
                  2.dapat berbagi penggunaan resource/aplikasi spesifik di dalam jaringan.
                               
    
    
    
