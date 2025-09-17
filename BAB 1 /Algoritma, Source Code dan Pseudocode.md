
 # 1.2 Algoritma, Source Code dan Pseudocode

## Algoritma 
Algoritma adalah Algoritma adalah serangkaian langkah atau prosedur logis yang digunakan untuk menyelesaikan suatu masalah secara sistematis. Kata algoritma berasal dari kata “Algoritmi”, yaitu nama latin dari matematikawan Persia bernama Abu Ja’far Muhammad Ibn Musa Al-Khawarizmi.

**Contoh**
<br/>
**Algoritma membuat teh**

```md
1. Rebus air hingga mendidih.
2. Siapkan gelas dan tuangkan air panas.
3. Celupkan kantong teh, tunggu beberapa menit hingga teh larut sempurna.
4. Tambahkan gula, aduk, dan teh siap dinikmati.
```
**Algoritma menentukan kelulusan**

```md
1. Ambil nilai ujian salah satu mahasiswa (dari console)
2. Jika nilai tersebut:
   - 75 ke atas, maka mahasiswa tersebut lulus (tampilkan ke console)
   - Kurang dari 75, maka mahasiswa tersebut harus menjalani remidiasi (tampilkan ke console)
```
## Pseudocode
Cara lain untuk **merepresentasikan suatu algoritma** adalah dalam bentuk **pseudocode**. Pseudocode pada dasarnya merupakan potongan kode yang menggunakan sintaks (aturan penulisan) yang **tidak formal** dengan tujuan memudahkan pembaca untuk memahami algoritmanya. Tidak ada batasan khusus dalam pembuatan pseudocode, asalkan mudah dimengerti dan dipahami saja oleh orang lain sehingga dapat mengetahui algoritma yang kita buat tanpa harus meraba-raba source codenya.

Berikut merupakan contoh pseudocode program 

```bash
Algoritma: TambahDuaAngka

  Deklarasi
    a: integer
    b: integer
    c: integer

  Algoritma
    Input a
    Input b
    c <- a + b
    Output c
```

Kemudian berikut merupakan contoh pseudocode program berdasarkan **Algoritma menentukan kelulusan**

```bash
Algoritma: CekNilaiUjian

  Deklarasi
    nilai: integer

  Algoritma
    Input nilai
    if nilai >= 75 then
      Output "Selamat!"
      Output "Anda dinyatakan lulus"
    else
      Output "Maaf!"
      Output "Anda harus mengikuti remidiasi"
    end if
```
## Source Code
Source code adalah teks atau kumpulan instruksi yang ditulis oleh programmer menggunakan bahasa pemrograman, menjadi dasar untuk menghasilkan program komputer atau aplikasi.

Dengan kata lain, source code merupakan representasi tertulis dari algoritma dan logika yang membentuk suatu program. Ini mencakup pernyataan, instruksi, dan struktur data yang bisa dibaca manusia dan dimengerti komputer. Berikut merupakan contoh source code program nilai kelulusan
```c
#include <stdio.h>

int main() {
  int nilaiMahasiswa;

  printf("Masukkan nilai anda: ");
  scanf("%d", &nilaiMahasiswa);

  if (nilaiMahasiswa >= 75) {
    printf("Selamat!\n");
    printf("Anda dinyatakan lulus\n");
  } else {
    printf("Maaf!\n");
    printf("Anda harus mengikuti remidiasi\n");
  }

  return 0;
}
```


