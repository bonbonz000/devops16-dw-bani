Question :

PART 1.
1. Jelaskan dan contohkan command untuk Text Manipulation!
2. Buatlah sebuah script untuk :
    - Memberikan akses ufw kepada port 22, 80, 443 dan 3000
    - Update apt dan install nginx

Answer :

1.
A.cat (concatenate) - berfungsi untuk display konten dari satu atau beberapa file 
tanpa harus editing full menggunakan tools seperti nano, vim. fungsi lainnya bisa 
untuk memasukan/menimpa text baru menggunakan ">" atau menambahkan text baru dengan ">>".
bisa digunakan juga untuk mengggabungkan dua file kedalam satu file baru.

Example :
	display |  cat nama_file
	addition replace | cat > nama_file
	addition new line |  cat >> nama_file
	merge | cat file1 file1 > file_baru

B.sed (stream editor) - berfungsi untuk melakukan manipulasi pada string/text pada 
sebuah file.

example :
	replace text | sed -i 's/apaantuh?/emangnya_apaan??/g' nama_file_target
keterangan :
	 -i menandakan edit file di tempat/secara direct
	 -s menandakan search
	 -g menandakan penerapan global

C.grep - berfungsi untuk melakukan pencarian spesifik di dalam sebuah file.

example ;
	pencarian string | grep -i nasbung_nastak nama_file
	penghitungan total string ditemukan | grep -i -c sundul_gans nama_file

D.sort - berfungsi untuk melakukan sortir terhadap suatu file.

example : 
	sorting default(ascending, angka terlebih dahulu) | sort nama_file
	sorting reverse (descending) | sort -r nama_file

E.echo - untuk print out string dari sebuah file, atau bis digunakan untuk addition 
replace atau addition new line string baru terhadap suatu file

example : 
	print out | echo "geser bang sempit" string addition new_line | echo string 
	addition replace | echo "geser bang sempit" > nama_file
	addition add line | echo "geser bang sempit" >> nama_file

2.custom script creation

![0](https://user-images.githubusercontent.com/91004163/227274212-08b66322-33a3-47eb-a182-204848b640de.png)

execute script (make sure sudo because UFW)

![1](https://user-images.githubusercontent.com/91004163/227273943-4e1ff9f0-99ab-439d-88a0-5bc8525e121c.png)


PART 2.

Question : 

1. Jelaskan tampilan dari htop!
2. Gunakan nmon untuk menampilkan CPU, RAM usage dan Network I/O!

Answer :

1.htop adalah tools untuk monitoring resource seperti cpu, memory, swap yang ada di 
perangkat yang memiliki sistem operasi linux.



keterangan

upper part:

CPU - menandakan kinerja CPU (1 dan 2 menandakan total core) warna biru 
(low priority), green (user), dan merah (kernel)

Mem - total penggunaan memory. 

Swp - Memory cadangan, jika aplikasi dalam posisi idle akan di serahkan ke 
memory swap 

Tasks - aplikasi yang sedang berjalan di server. format : task, threads, dan current 
running

Load average - rata-rata aplikasi yang berjalan. format : last 1, 5 dan periode 15 menit

Uptime - berapa lama server sudah berjalan. 

lower part:

PID - nomor proses id setiap proses yang berjalan di linux. 

USER - nama user dari proses tersebut

PRI - kernel-space priority of processess. dari range 0 - 139

NI - niceness atau user space priority. dari range -20(tertinggi) sampai 19 (terendah)

VIRT - total virtual memory yang di request oleh proses

RES - resident memory usage ( apa yang sedang di gunakan oleh prosesnya)

SHR - shred memory yang dipakai oleh proses

S - persentase CPU yang sedang di gunakan

MEM% - share dari memori(ram) yang digunakan oleh task. RES di bagi total memory

TIME+ - waktu dari prosesor yang di gunakan oleh proses

Command - perintah apa yang sedang di jalankan.

f1 - digunakan untuk melihat help
