Pemrograman Lanjut (Advanced Programming) 2024/2025 Genap
* Nama    : Priscilla Natanael Surjanto
* NPM     : 2306152153
* Kelas   : Pemrograman Lanjut - A

## Before Optimization
 
### Test Plan 1 - all-student request (GUI)
![Screenshot (75)](https://github.com/user-attachments/assets/8b300925-7142-438d-85fd-a9252fd17e76)
 
### Test Plan 1 - all-student request (JTL)
![image](https://github.com/user-attachments/assets/ae51bbc9-a13f-41af-9760-851729e569a6)

### Test Plan 2 - all-student-name request (GUI)
![Screenshot (74)](https://github.com/user-attachments/assets/0450881f-fd6c-41d4-8617-65cd9ba57421)

### Test Plan 2 - all-student-name request (JTL)
![image](https://github.com/user-attachments/assets/efbd0cae-7429-4639-a2a7-b3edd025b576)

### Test Plan 3 - highest-gpa request (GUI)
![Screenshot (73)](https://github.com/user-attachments/assets/6e8fa219-d679-45ec-bfe0-16994a8f3ac5)

### Test Plan 3 - highest-gpa request (JTL)
![image](https://github.com/user-attachments/assets/c44b4f14-d24f-40da-ba6b-c1e411bac153)

## After Optimization

### Test Plan 1 - all-student request (GUI)
![Screenshot (78)](https://github.com/user-attachments/assets/da2f78fe-d662-4ea9-93d6-2e74a3cb1b1a)

### Test Plan 1 - all-student request (JTL)
![image](https://github.com/user-attachments/assets/15f8ac6c-dcff-4f28-b400-c044922015a4)

### Test Plan 2 - all-student-name request (GUI)
![Screenshot (79)](https://github.com/user-attachments/assets/8902783f-7109-41df-94dd-f34afb429511)

### Test Plan 2 - all-student-name request (JTL)
![image](https://github.com/user-attachments/assets/62dd7cdd-5a00-4fd7-88b5-b7104c477949)

### Test Plan 3 - highest-gpa request (GUI)
![Screenshot (80)](https://github.com/user-attachments/assets/b56add35-91b3-4007-8a75-c76b8d63f3e7)

### Test Plan 3 - highest-gpa request (JTL)
![image](https://github.com/user-attachments/assets/e31bc107-9547-49de-9bd2-a32100f1490f)

## Kesimpulan
- all-student
  - Sebelum melakukan optimisasi, sample time untuk sample ke-10 adalah 525759ms.
  - Setelah melakukan optimisasi, sample time untuk sample ke-10 adalah 13571ms.
  - Maka, terjadi speedup sebesar 38.74x lebih cepat.


- all-student-name
  - Sebelum melakukan optimisasi, sample time untuk sample ke-10 adalah 18058ms.
  - Setelah melakukan optimisasi, sample time untuk sample ke-10 adalah 1693ms.
  - Maka, terjadi speedup sebesar 10.67x lebih cepat.


- highest-gpa
  - Sebelum melakukan optimisasi, sample time untuk sample ke-10 adalah 180ms.
  - Setelah melakukan optimisasi, sample time untuk sample ke-10 adalah 12ms.
  - Maka, terjadi speedup sebesar 15x lebih cepat.

## Refleksi

1. Apa perbedaan pendekatan pengujian performa dengan JMeter dan profiling dengan IntelliJ Profiler dalam konteks optimasi performa aplikasi?


   - Jika menggunakan JMeter, maka performa aplikasi diuji dari perspektif eksternal dengan melakukan simulasi beban pengguna dan mengukut metrik seperti response time, throughput, dan error rate.
   - Jika menggunakan IntelliJ Profiler, maka analisis performa lebih terfokus pada internal aplikasi, yaitu penggunaan CPU, memory allocation, dan metode mana yang memakan waktu lama.
   - JMeter lebih cocok untuk mengukur kinerja sistem di bawah beban, sedangkan IntelliJ Profiler membantu mengidentifikasi hambatan di tingkat kode.


2. Bagaimana proses profiling membantu dalam mengidentifikasi dan memahami titik lemah dalam aplikasi?

Dengan menjalani proses profiling, data rinci mengenai penggunaan sumber daya oleh aplikasi diberikan. Setelah data tersebut dianalisis, maka kita bisa mengetahui metode atau bagian kode mana yang bisa dioptimalkan untuk meningkatkan efisiensi aplikasi.

3. Apakah IntelliJ Profiler efektif dalam membantu menganalisis dan mengidentifikasi bottleneck dalam kode aplikasi?

Menurut saya, IntelliJ Profiler cukup efektif karena hasil analisis langsung terdapat pada IDE dengan tampilan visual yang intuitif, isi analisis laporan pemakaian CPU dan memori yang detail, sehingga mudah saya pahami. Dengan data yang didapat dari IntelliJ Profiler, saya bisa langsung menelusuri bagian kode yang bisa dioptimalkan agar aplikasi saya bisa lebih efektif.

4. Apa tantangan utama yang dihadapi saat melakukan pengujian performa dan profiling, serta bagaimana cara mengatasinya?

Tantangan utama yang saya hadapi saat melakukan pengujian performa, yaitu memahami hasil analisis data dari profiling, terutama karena saya baru pertama kali melakukan profiling. Cara saya mengatasinya, yaitu saya melakukan research dari internet dan menggunakan dokumentasi serta referensi dari IntelliJ Profiler sebagai panduan.

5. Apa manfaat utama dari penggunaan IntelliJ Profiler untuk profiling kode aplikasi?

Manfaat utama dari penggunaan IntelliJ Profiler untuk profiling kode aplikasi, yaitu alat ini sudah terintegrasi dengan IDE sehingga sangat mudah mengidentifikasi metode atau bagian kode yang menyebabkan aplikasi tereksekusi dengan lama. Hanya dengan satu klik, saya bisa langsung diarahkan ke bagian kode tersebut untuk proses optimalisasi. Selain itu, waktu sample juga tertera di samping bagian kode tersebut, sehingga saya bisa mendapatkan pemahaman yang lebih mendalam tentang penggunaan CPU dan memori.

6. Bagaimana menangani situasi di mana hasil profiling dengan IntelliJ Profiler tidak sepenuhnya konsisten dengan temuan dari pengujian performa menggunakan JMeter?

Dalam situasi di mana hasil profiling di IntelliJ Profiler tidak konsisten dengan hasil JMeter, maka saya akan melakukan pengecekan ulang pada skenario pengujian di JMeter mengenai apakah beban yang diberikan sudah realistis. Lalu, saya akan menjalankan profiling dengan beberapa skenario berbeda untuk melihat pola atau faktor apa yang mempengaruhi variasi hasil tersebut.  

7. Strategi apa yang diterapkan dalam mengoptimalkan kode aplikasi setelah menganalisis hasil dari pengujian performa dan profiling? Bagaimana memastikan perubahan yang dilakukan tidak mempengaruhi fungsionalitas aplikasi?

   - Strategi yang saya terapkan, yaitu saya memanfaatkan repository untuk query yang lebih efisien dalam metode `findStudentWithHighestGpa()`, menggunakan `StringBuilder` untuk menggabungkan string dalam metode `joinStudentNames()`, dan hanya me-return `studentCourseRepository.findAll()` pada metode `getAllStudentsWithCourses()` sebab fitur `findAll()` dari Spring Data JPA.
   - Cara saya memastikan perubahan yang dilakukan tidak memengaruhi fungsionalitas aplikasi, yaitu melakukan pengujian kode secara menyeluruh setelah terdapat perubahan.