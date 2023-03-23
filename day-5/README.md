Question :
1. Jelaskan dan contohkan command untuk Text Manipulation!
2. Buatlah sebuah script untuk :
    - Memberikan akses ufw kepada port 22, 80, 443 dan 3000
    - Update apt dan install nginx

Answer :

1.cat (concatenate) - berfungsi untuk display konten dari satu atau beberapa file 
tanpa harus editing full menggunakan tools seperti nano, vim. fungsi lainnya bisa 
untuk memasukan/menimpa text baru menggunakan ">" atau menambahkan text baru dengan ">>".
bisa digunakan juga untuk mengggabungkan dua file kedalam satu file baru.

Example :
	display |  cat nama_file
	addition replace | cat > nama_file
	addition new line |  cat >> nama_file
	merge | cat file1 file1 > file_baru

sed (stream editor) - berfungsi untuk melakukan manipulasi pada string/text pada 
sebuah file.

example :
	replace text | sed -i 's/apaantuh?/emangnya_apaan??/g' nama_file_target
keterangan :
	 -i menandakan edit file di tempat/secara direct
	 -s menandakan search
	 -g menandakan penerapan global

grep - berfungsi untuk melakukan pencarian spesifik di dalam sebuah file.

example ;
	pencarian string | grep -i nasbung_nastak nama_file
	penghitungan total string ditemukan | grep -i -c sundul_gans nama_file

sort - berfungsi untuk melakukan sortir terhadap suatu file.

example : 
	sorting default(ascending, angka terlebih dahulu) | sort nama_file
	sorting reverse (descending) | sort -r nama_file

echo - untuk print out string dari sebuah file, atau bis digunakan untuk addition 
replace atau addition new line string baru terhadap suatu file

example : 
	print out | echo "geser bang sempit" string addition new_line | echo string 
	addition replace | echo "geser bang sempit" > nama_file
	addition add line | echo "geser bang sempit" >> nama_file

