# 1.1 - Pengantar (Program Sederhana, Variabel, dan Input/Output) 
# contoh program sederhana
```c
// menambahkan library stdio.h
#include <stdio.h>

int main() {
  printf("Hello world!");
  return 0;
}
```
#Bagaimana Memahami Program diatas ?

```c
#include <stdio.h>
```
```Include stdio.h``` adalah sebuah kode pada bahasa pemrograman ```C``` untuk mengakses library standard input dan output file. 
Kode tersebut terdiri dari 2 kode yang menjadi satu yakni ```include``` dan juga ```stdio.h```. `stdio.h` merupakan library 
bawaan bahasa C yang di dalamnya terdapat banyak fungsi, salah satunya adalah fungsi `printf()`. Oleh karena itu, 
ketika kita ingin menggunakan fungsi `printf()` diharuskan untuk menggunakan library `stdio.h`.
> Notes :
> Baris kode ```#include <stdio.h>``` dan pendefinisian library lainya disebut dengan preprocessor directive. Baris kode tersebut berbeda dengan baris kode C lainya.
> Preprocessor directive tidak memerlukan titik koma ( ; ) pada akhir barisnya.
<br />

```c
 int main(){
 //..Kode..///
}
```
kode di atas adalah fungsi ```main()``` atau fungsi utama dalam sebuah program C. Fungsi ```main``` tersebut akan dijalankan pertama kali ketika sebuah program C dijalankan. 
Sebelum fungsi ```main``` terdapat inialisasi `int` yang menandakan return value dari fungsi tersebut bertipe `int` atau bilangan bulat.
> Notes :
> Pembahasan mengenai ```function``` atau fungsi serta return value akan dibahas pada pertemuan mendatang.
<br/>






