# <h1 align="center">Laporan Praktikum Modul 2 - PENGENALAN BAHASA C++ (BAGIAN KEDUA)</h1>
<p align="center">Zuhra Hanani Ramadhina - 109082500143</p>

## Dasar Teori

Array merupakan struktur data yang menyimpan sekumpulan elemen dengan tipe data sama dalam satu blok memori yang berurutan, di mana setiap elemen dapat diakses menggunakan indeks[1]. Array dapat berbentuk satu dimensi maupun multidimensi (seperti matriks dua dimensi), tergantung kebutuhan penyimpanan data. Selain array, konsep pointer juga menjadi dasar penting dalam pemrograman C++, yaitu variabel yang menyimpan alamat memori dari variabel lain, sehingga memungkinkan manipulasi data secara langsung melalui alamat tersebut[2].

### A. Array Multidimensi<br/>
Array multidimensi adalah array yang memiliki lebih dari satu indeks, digunakan untuk merepresentasikan data dalam bentuk tabel, matriks, atau struktur berlapis lainnya. Array dua dimensi umum digunakan untuk merepresentasikan matriks, sedangkan array tiga dimensi atau lebih digunakan untuk data yang lebih kompleks seperti data bertingkat.

#### 1. Array satu dimensi — menyimpan data dalam satu baris indeks
#### 2. Array dua dimensi (matriks) — menyimpan data dalam bentuk baris dan kolom
#### 3. Array tiga dimensi dan empat dimensi — menyimpan data berlapis dengan beberapa indeks

### B. Pointer dan Reference<br/>
Pointer adalah variabel yang menyimpan alamat memori dari variabel lain, dilambangkan dengan operator `*` untuk deklarasi dan dereference, serta operator `&` untuk mengambil alamat suatu variabel[2]. Reference merupakan alias atau nama lain dari suatu variabel yang sudah ada, sehingga perubahan pada reference akan langsung memengaruhi variabel aslinya tanpa perlu dereference eksplisit.

#### 1. Operator `&` — mengambil alamat memori suatu variabel
#### 2. Operator `*` — mengakses nilai yang ditunjuk oleh pointer (dereference)
#### 3. Reference (`&` pada parameter fungsi) — alias variabel yang memungkinkan fungsi memodifikasi nilai asli

## Guided 

### 1. Array 1

```C++
#include <iostream>
using namespace std;

int main() {
    int nilai[5];

    nilai[0] = 80;
    nilai[1] = 85;
    nilai[2] = 90;
    nilai[3] = 75;
    nilai[4] = 95;

    for (int i = 00; i < 5; i++) {
        cout << "index ke-" << i << " = " << nilai[i] << endl;

    }

    return 0;
}
```
Program mendeklarasikan array 1 dimensi nilai[5], lalu mengisi tiap indeksnya secara manual dengan nilai tertentu. Perulangan for digunakan untuk menampilkan seluruh isi array beserta nomor indeksnya.

### 2. Array 2

```C++
#include <iostream>
using namespace std;

int main() {
    int nilai[3][3] = {
        {70, 85, 90},
        {75, 80, 85},
        {90, 95, 100}
    };

    // for (int i = 0; i < 3; i++) {
    //     for (int j = 0; j < 3; j++) {
    //         cout << nilai[i][j] << " ";
    //     }
    //     cout << endl;
    // }

    cout << nilai[0][0] << endl; //80
    cout << nilai[1][1] << endl; //80
    cout << nilai[2][2] << " "; //100

    return 0;
}
```
Program mendeklarasikan array 2 dimensi (matriks 3x3) yang langsung diinisialisasi nilainya saat deklarasi. Elemen diagonal diakses langsung menggunakan indeks baris dan kolom yang sama (nilai[0][0], nilai[1][1], nilai[2][2]), menghasilkan 70, 80, dan 100.

### 3. Array 3

```C++
#include <iostream>
using namespace std;

int main() {
    int data[2][3][3] = {
        {
            {1, 2, 3},
            {4, 5, 6},
            {7, 8, 9}
        },
        {
            {10, 11, 12},
            {13, 14, 15},
            {16, 17, 18}
        }
    };

    // for (int i = 0; i < 2; i++) {
    //     for (int j = 0; j < 3; j++) {
    //         for (int k = 0; k < 3; k++) {
    //             cout << data[1][j][k] << " ";
    //         }
    //        cout << endl;
    //      }
    //     cout << endl;
    // }

    cout << data[0][1][1] << " "; //5

    return 0;
}
```
Program mendeklarasikan array 3 dimensi data[2][3][3], yaitu kumpulan 2 buah matriks 3x3. Elemen data[0][1][1] mengakses matriks pertama (indeks 0), baris ke-1, kolom ke-1, yang menghasilkan nilai 5.

### 4. Array 4

```C++
#include <iostream>
using namespace std;

int main() {
    int data[2][2][2][2] = {
        {
            {
                {1, 2},
                {3, 4}
            },
            {
                {5, 6},
                {7, 8}
            }
        },
        {
            {
                {9, 10},
                {11, 12}
            },
            {
                {13, 14},
                {15, 16}
            }
        }
    };

    cout << data[0][0][0][0] << endl; //1
    cout << data[1][1][1][1] << endl; //16

    return 0;
}
```
Program mendeklarasikan array 4 dimensi data[2][2][2][2]. Elemen data[0][0][0][0] mengambil nilai pertama (1), sedangkan data[1][1][1][1] mengambil nilai terakhir dari struktur bersarang tersebut (16), menunjukkan cara penelusuran array berdimensi banyak.

### 5. Pointer 1

```C++
#include <iostream>
using namespace std;

int main() {
    char a;
    int j;
    char arr[6];

    arr[3] = 'b';
    a = 'u';
    j = 10;

    cout << a << endl;
    cout << &a << endl;

    cout << j << endl;
    cout << &j << endl;

    cout << arr[3] << endl;
    cout << &(arr[4]) << endl;
    
    return 0;
}
```
Program mendeklarasikan variabel char, int, dan array char, lalu menampilkan nilai variabel menggunakan operator biasa (a, j, arr[3]) serta alamat memorinya menggunakan operator & (&a, &j, &(arr[4])). Ini menunjukkan perbedaan antara mengakses nilai dan mengakses alamat memori suatu variabel.

### 6. Pointer 2

```C++
#include <iostream>
using namespace std;

int main() {
    int x, y;
    int *px;

    x = 87;
    px = &x;
    y = *px;

    cout << "Alamat x= " << &x << endl;
    cout << "Isi px= " << px << endl;
    cout << "Isi x= " << x << endl;
    cout << "Nilai yang ditunjuk px= " << *px << endl;
    cout << "Nilai y= " << y << endl;

    return 0;
}
```
Program mendemonstrasikan penggunaan pointer dasar. Variabel px menyimpan alamat dari x (px = &x), sehingga *px (dereference) menghasilkan nilai yang sama dengan x. Nilai tersebut kemudian disalin ke variabel y.

### 7. Pointer 3

```C++
#include <iostream>
#define MAX 5
using namespace std;

int main() {
    int i, j;
    float nilai_total, rata_rata;
    float nilai[MAX];

    static int nilai_tahun[MAX][MAX] = {
        {0, 2, 2, 0, 0},
        {0, 1, 1, 1, 0},
        {0, 3, 3, 3, 0},
        {4, 4, 0, 0, 4},
        {5, 0, 0, 0, 5}
    };

    // inisialisasi array satu dimensi
    for (i = 0; i < MAX; i++) {
        cout << "masukan nilai ke-" << i + 1 << endl;
        cin >> nilai[i];
    }

    cout << "\ndata nilai siswa :\n";

    // menampilkan array satu dimensi
    for (i = 0; i < MAX; i++)
        cout << "nilai k-" << i + 1 << "=" << nilai[i] << endl;

    cout << "\n nilai tahunan : \n";

    // menampilkan array dua dimensi
    for (i = 0; i < MAX; i++) {
        for (j =  0; j <MAX; j++)
            cout << nilai_tahun[i][j];

        cout << "\n";
    }

    return 0;
}
```
Program menggabungkan array 1 dimensi (nilai) yang diisi melalui input pengguna dan array 2 dimensi statis (nilai_tahun) yang sudah diinisialisasi. Program menampilkan keduanya menggunakan perulangan for, mendemonstrasikan kombinasi input dinamis dan data statis dalam satu program.

### 8. Pointer 4

```C++
#include <iostream>
using namespace std;

int main() {
    char nama[] = "strukdat";

    cout << nama << endl;
    cout << nama[3] << endl;

    return 0;
}
```
Program mendeklarasikan array char yang diisi dengan string "strukdat". Karena string di C++ sebenarnya adalah array karakter, nama dapat ditampilkan langsung sebagai teks penuh, sedangkan nama[3] mengakses karakter tunggal pada indeks ke-3 (yaitu 'k').

## Unguided 

### 1. Buatlah program yang dapat melakukan operasi penjumlahan, pengurangan, dan perkalian matriks 3x3 

```C++
#include <iostream>
using namespace std;

int main() {
    int A[3][3], B[3][3], hasil[3][3];

    cout << "Masukkan elemen matriks A:" << endl;
    for (int i = 0; i < 3; i++)
        for (int j = 0; j < 3; j++) {
            cout << "A[" << i << "][" << j << "] = ";
            cin >> A[i][j];
        }

    cout << "Masukkan elemen matriks B:" << endl;
    for (int i = 0; i < 3; i++)
        for (int j = 0; j < 3; j++) {
            cout << "B[" << i << "][" << j << "] = ";
            cin >> B[i][j];
        }

    //penjumlahan
    cout << "\nHasil penjumlahan A + B:" << endl;
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            hasil[i][j] = A[i][j] + B[i][j];
            cout << hasil[i][j] << " ";
        }
        cout << endl;
    }

    //pengurangan
    cout << "\nHasil pengurangan A - B:" << endl;
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            hasil[i][j] = A[i][j] - B[i][j];
            cout << hasil[i][j] << " ";
        }
        cout << endl;
    }

    //perkalian
    cout << "\nHasil perkalian A x B:" << endl;
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            hasil[i][j] = 0;
            for (int k = 0; k < 3; k++)
                hasil[i][j] += A[i][k] * B[k][j];
            cout << hasil[i][j] << " ";
        }
        cout << endl;
    }

    return 0;
}
```
### Output Unguided 1 :

##### Output
![Screenshot Output Unguided 1](https://github.com/oreoceese/laprak2-struktur-data/blob/main/2-soal1.png)

Program menerima input dua matriks 3x3 dari pengguna (A dan B), lalu melakukan tiga operasi menggunakan perulangan bersarang (nested loop): penjumlahan dan pengurangan dilakukan dengan menjumlah/mengurangkan elemen yang posisinya sama, sedangkan perkalian matriks menggunakan rumus perkalian baris-kolom (setiap elemen hasil didapat dari penjumlahan hasil kali elemen baris A dengan kolom B, memakai loop ketiga sebagai akumulator).

### 2. Berdasarkan guided pointer dan reference sebelumnya, buatlah keduanya dapat menukar nilai dari 3 variabel

```C++
#include <iostream>
using namespace std;

void tukarPointer(int *a, int *b, int *c) {
    int temp = *a;
    *a = *b;
    *b = *c;
    *c = temp;
}

void tukarReference(int &a, int &b, int &c) {
    int temp = a;
    a = b;
    b = c;
    c = temp;
}

int main() {
    int x, y, z;
    cout << "Masukkan nilai x, y, z: ";
    cin >> x >> y >> z;

    cout << "\nSebelum ditukar: x=" << x << " y=" << y << " z=" << z << endl;

    // pake pointer
    int x1 = x, y1 = y, z1 = z;
    tukarPointer(&x1, &y1, &z1);
    cout << "Setelah ditukar (pointer): x=" << x1 << " y=" << y1 << " z=" << z1 << endl;

    // pake reference
    int x2 = x, y2 = y, z2 = z;
    tukarReference(x2, y2, z2);
    cout << "Setelah ditukar (reference): x=" << x2 << " y=" << y2 << " z=" << z2 << endl;

    return 0;
}
```
### Output Unguided 2 :

##### Output
![Screenshot Output Unguided 2](https://github.com/oreoceese/laprak2-struktur-data/blob/main/2-soal2.png)

Program ini menukar nilai tiga variabel dengan pola rotasi satu arah, di mana setiap variabel menerima nilai dari variabel berikutnya, dan variabel terakhir menerima nilai awal dari variabel pertama yang disimpan sementara dalam `temp`. Kedua pendekatan, baik menggunakan pointer (`*a`, `*b`, `*c`) maupun reference (`&a`, `&b`, `&c`), menghasilkan output yang identik karena keduanya memungkinkan fungsi memodifikasi nilai variabel asli di luar lingkup fungsi, bukan hanya salinannya.

### 3. Buatlah program yang dapat mencari nilai minimum, maksimum, dan rata – rata dari array tersebut! Gunakan function cariMinimum() untuk mencari nilai minimum dan function cariMaksimum() untuk mencari nilai maksimum, serta gunakan prosedur hitungRataRata() untuk menghitung nilai rata – rata!

```C++
#include <iostream>
using namespace std;

int arrA[] = {11, 8, 5, 7, 12, 26, 3, 54, 33, 55};
int n = 10;

void tampilkanArray() {
    cout << "Isi array: ";
    for (int i = 0; i < n; i++) cout << arrA[i] << " ";
    cout << endl;
}

int cariMaksimum() {
    int maks = arrA[0];
    for (int i = 1; i < n; i++)
        if (arrA[i] > maks) maks = arrA[i];
    return maks;
}

int cariMinimum() {
    int min = arrA[0];
    for (int i = 1; i < n; i++)
        if (arrA[i] < min) min = arrA[i];
    return min;
}

void hitungRataRata() {
    int total = 0;
    for (int i = 0; i < n; i++) total += arrA[i];
    float rata = (float)total / n;
    cout << "Rata-rata: " << rata << endl;
}

int main() {
    int pilihan;

    do {
        cout << "\n--- Menu Program Array ---" << endl;
        cout << "1. Tampilkan isi array" << endl;
        cout << "2. Cari nilai maksimum" << endl;
        cout << "3. Cari nilai minimum" << endl;
        cout << "4. Hitung nilai rata-rata" << endl;
        cout << "0. Keluar" << endl;
        cout << "Pilihan: ";
        cin >> pilihan;

        switch (pilihan) {
            case 1:
                tampilkanArray();
                break;
            case 2:
                cout << "Nilai maksimum: " << cariMaksimum() << endl;
                break;
            case 3:
                cout << "Nilai minimum: " << cariMinimum() << endl;
                break;
            case 4:
                hitungRataRata();
                break;
            case 0:
                cout << "Keluar program." << endl;
                break;
            default:
                cout << "Pilihan tidak valid." << endl;
        }
    } while (pilihan != 0);

    return 0;
}
```
### Output Unguided 3 :

##### Output 1
![Screenshot Output Unguided 3_1](https://github.com/oreoceese/laprak2-struktur-data/blob/main/2-soal3.png)

##### Output 2
![Screenshot Output Unguided 3_2](https://github.com/oreoceese/laprak2-struktur-data/blob/main/2-soal3_2.png)

Program menggunakan array global arrA yang sudah ditentukan, dengan tiga fungsi terpisah: cariMinimum() dan cariMaksimum() menelusuri array sambil membandingkan tiap elemen untuk menemukan nilai ekstrem, sedangkan hitungRataRata() menjumlahkan seluruh elemen lalu membaginya dengan jumlah data. Struktur switch-case di dalam do-while membuat menu terus muncul berulang sampai pengguna memilih keluar (input 0).

## Kesimpulan

Berdasarkan praktikum yang telah dilakukan, dapat disimpulkan bahwa array merupakan struktur data penting dalam C++ untuk menyimpan dan mengelola sekumpulan data sejenis, baik dalam bentuk satu dimensi maupun multidimensi seperti matriks. Penguasaan konsep pointer dan reference juga sangat penting karena keduanya memungkinkan program untuk memanipulasi nilai variabel secara langsung melalui alamat memori, yang berguna terutama saat menukar nilai antar variabel atau mengirim data ke dalam fungsi tanpa menyalin nilainya. Selain itu, melalui latihan guided dan unguided, mahasiswa dilatih menerapkan operasi matriks, pertukaran nilai menggunakan pointer dan reference, serta pembuatan program menu interaktif menggunakan struktur switch-case untuk mengolah data array.

## Referensi
[1] Triase. (2020). Diktat Edisi Revisi : STRUKTUR DATA. Medan: UNIVERSTAS ISLAM NEGERI SUMATERA UTARA MEDAN.
<br>[2] Indahyanti, Uce., Rahmawati, Yunianita. (2020). *Buku Ajar Algoritma dan Pemrograman dalam Bahasa C++*. Sidoarjo: UMSIDA Press. Diakses melalui https://doi.org/10.21070/2020/978-623-6833-67-4.
