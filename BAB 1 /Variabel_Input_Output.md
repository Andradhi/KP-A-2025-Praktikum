# 1.1 - Pengantar (Variabel, input dan Output) 
contoh program sederhana
```c
// menambahkan library stdio.h
#include <stdio.h>

int main() {
  printf("Hello world!");
  return 0;
}
```
Bagaimana Memahami Program diatas ?

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

```c
  printf("Hello World!");
```
Dalam bahasa C, fungsi ```printf()``` digunakan untuk mencetak keluaran yang diformat dalam banyak cara ke keluaran standar stdout. Pada umunya dicetak dalam format konsol.
Untuk menggunakan fungsi ini, kita dapat menuliskan apa yang ingin kita cetak dalam parameter fungsi.
> notes : 
> Parameter merupakan variabel yang akan digunakan untuk menampung data
<br/>

```c
return 0 ;
```
Fungsi ```return``` berfungsi untuk menghentikan sebuah fungsi, dalam kasus ini fungsi ```return``` menghentikan fungsi ```main``` serta mengembalikan data ke pemanggil fungsi. Karena ```main``` adalah fungsi utama maka ```return``` akan menghentikan program. Angka `0` setelah fungsi ```return``` adalah sebuah konvensi standar yang menandakan keberhasilan program.
```c
// menambahkan library stdio.h
/*
  komentar dengan 2 atau lebih
  baris
 */
```
kode diatas tidak akan dijalankan oleh program. Cara menggunakanya dengan inialisasi ```//``` untuk single line atau menggunakan ```/*........*/``` untuk multi line.
## Variabel dan Tipe Data
Apa itu variabel ?
Variabel adalah tempat menyimpan sebuah nilai. Sementara tipe data adalah jenis nilai yang akan tersimpan dalam variabel.
contoh variabel
```c
  umur = 18 ; //variabel umur dengan nilai 18
  jumlah_kemenangan = 12 ; //variabel dengan nama jumlah_kemenangan dengan nilainya 12
```
Tipe data dibagi menjadi beberapa jenis yaitu tipe data integer, floating point dan char.
1. Tipe data Integer
   <br/>
Tipe data integer merupakan kumpulan bilangan bulat. Integer adalah semua bilangan bulat termasuk nol (0), bilangan positif maupun negatif yang tidak memiliki angka desimal (angka di belakang koma).

| Tipe Data  | Ukuran (bytes) | Range                             | Format Specifier |
|------------|----------------|-----------------------------------|------------------|
| short      | 2              | -32,768 to 32,767                 | %hd              |
| unsigned short | 2          | 0 to 65,535                       | %hu              |
| int        | 4              | -2,147,483,648 to 2,147,483,647   | %d               |
| unsigned int | 4            | 0 to 4,294,967,295                | %u               |
| long       | 4              | -2,147,483,648 to 2,147,483,647   | %ld              | 
| unsigned long | 4           | 0 to 4,294,967,295                | %lu              |
| long long  | 8              | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 | %lld |
| unsigned long long | 8      | 0 to 18,446,744,073,709,551,615   | %llu             |

2. Tipe data floating point
   <br/>
Tipe data ini merupakan kumpulan bilangan real (pecahan desimal).

| Tipe Data | Ukuran (bytes) | Range (approx)                        | Format Specifier |
|-----------|----------------|---------------------------------------|------------------|
| float     | 4              | ±1.2E-38 to ±3.4E+38                  | %f               |
| double    | 8              | ±2.3E-308 to ±1.7E+308                | %lf              |
| long double | 10 / 12 / 16 (tergantung compiler) | ±3.4E-4932 to ±1.1E+4932 | %Lf |

3. Tipe data Char
   <br/>
Sebuah variabel bertipedata char hanya dapat menampung satu karakter saja, tidak akan dapat menyimpan lebih dari satu karakter. Berikut ini adalah yang termasuk dalam tipe data char beserta ukurannya dalam satuan byte pada mesin 16 bit.

| Tipe Data | Ukuran (bytes) | Range         | Format Specifier |
|-----------|----------------|---------------|------------------|
| char      | 1              | -128 to 127   | %c               |
| unsigned char | 1          | 0 to 255      | %c               |
| signed char   | 1          | -128 to 127   | %c               |

### pendefinisian variabel 
Variabel-variabel yang akan digunakan pada program bahasa C harus didefinisikan terlebih dahulu sebelum digunakan. Contoh, kita ingin mendefinisikan variabel bernama `jumlahApel` dan `jumlahJeruk` dengan nilai 11 dan 10. Karena 11 dan 10 merupakan bilangan bulat, maka kita bisa menggunakan tipe data `int` sehingga penulisannya adalah seperti berikut.

```c
  int jumlahApel = 11 ;
  int jumlahJeruk = 10 ;
```
atau kita dapat mendefinisikan sebagai berikut:

```c
  int jumlahApel = 11, jumlahJeruk =  10 ;
```
kemudian jika kita ingin membuat sebuah variabel dengan nilai phi (3.14) dapat kita gunakan tipe data `float` dengan penulisan sebagai berikut:

```c
 float phi = 3.14 ;
```
## Input dan Output
input adalah data atau instruksi yang dimasukkan ke dalam program oleh pengguna atau sumber eksternal, sementara output adalah data atau hasil yang dikeluarkan oleh program setelah memproses input tersebut. 
### Output
Fungsi yang sudah kita pelajari untuk mencetak sebuah hasil atau keluaran sampai saat ini adalah fungsi `printf()`. Dengan contoh sebagai berikut:
```c
printf(" Hello World ") ;
printf(" Universitas Sebelas Maret ");
```
Kita juga dapat mencetak variabel yang kita ingginkan menggunakan format yang telah kita pelajari. Berikut contohnya :
```c
#include <stdio.h>
int main(){
    int umur =  19 ;
    char nama[30] = "Andradhi Bondan" ;
    char kelas = 'B' ;
    short semester = 3 ;

    printf("Perkenalkan nama saya %s dari kelas %c semester %hd dan berumur %d", nama, kelas, semester,umur) ;
    return 0 ;
}
```
output dari program di atas akan sebagai berikut :
```bash
Perkenalkan nama saya Andradhi Bondan dari kelas B semester 3 dan berumur 19
```
### Basic Input
Input dalam bahasa C dapat menggunakan fungsi `scanf`, input adalah data atau instruksi yang dimasukkan ke dalam program oleh pengguna.
```c
  scanf("%d", &angka) ;
  //.....///
  scanf("%s", &nama) ;
```
Penggunaan  dari fungsi input sebagai berikut:
```c
#include <stdio.h>
int main(){
    int umur ;
    short semester ;
    char nama[32] ;

    printf("Masukan Nama : ");
    scanf("%s", nama) ;
    printf("Masukan umur : ");
    scanf("%d", &umur) ;
    printf("Semester : ");
    scanf("%hd", &semester);

    printf("Nama anda adalah %s umur anda sekarang %d dan sedang berada di semester %hd", nama, umur, semester) ;
    return 0 ;
}
```
Kode ini akan menerima 3 masukan yang akan ditampung dalam beberapa variabel seperti nama, umur dan semester. Setelah user memberikan inputan, program akan mencetak hasilnya menggunakan fungsi `printf`. Penggunaan `scanf` Diperlukan ampersand ( & ) di depan variabel dengan tipe data integer/floating point. Namun, fungsi `scanf` memiliki kekurangan besar yaitu tidak bisa menerima string yang ber-spasi.







