Implementasi Algoritma Pembentuk Lingkaran dengan Algoritma Midpoin

Dalam project ini menggunakan Aplikasi CodeBlock sebagai tempat penulisan codingnya.
agar dapat menjalankan Project ini Codeblocknya harus sudah di include glut.h di MINGW -nya.
untuk cara include glut.h dapat dilihat di video ini : https://youtu.be/pak-Z6uQjAQ.

Algoritma MidPoint adalah suatu algoritma yang digunakan menggambar Lingkaran.
Dalam menggambar lingkaran kita harus menentukan jari2, dan titik pusat(Xc,Yc) dahulu.
dalam awal penentuan garis, titik pusat di set(0,0) setelah menentukan garisnya baru di translasi 
ke (Xc,Xy) 

Project ini menggunakan user input dalam menentukan jari2(r) dan titik pusatnya (x2,y2),
dengan catatan semua nilai harus positif.

Output program ini berupa garis yang digambar di window baru dan panjangnya sesuai dengan input.

Algoritma MidPoint yang digunakan :

1. Input r dan titik tengah lingkaran (xc,yc) dan posisi start awal (x0,y0) = (0,r)
2. Hitung p awal  (p=1-r)
3. Untuk tiap xk, k=0, ulangi sampai x <= y
   - Jika pk < 0, (xk+1,yk), pk+1=pk+2xk+1+1
   - Jika tidak, (xk+1,yk-1), pk+1=pk+2(xk+1-yk+1) + 1 
4. Tentukan titik simetri di tujuh oktan yang lain 
5. Pindahkan semua titik pixel (x,y) ke posisi dengan pusat (xc,yc) 
   - x=x+xc
   - y=y+yc
