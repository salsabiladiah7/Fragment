# Fragment
>Fragment adalah sebuah reuseable class yang mengimplement beberapa fitur sebuah Activity. Fragment biasanya dibuat sebagai bagian dari suatu antarmuka. Sebuah fragment harus berada di dalam sebuah activity, mereka tidak dapat berjalan sendiri tanpa adanya activity tempat mereka menempel.
Kelebihan yang didapatkan bila menggunakan fragment adalah sebagai berikut:
- Tidak perlu memasukkan nama file fragment ke dalam “AndroidManifest” yang diperlukan oleh activity.
- Fungsi yang berada pada activity dapat langsung digunakan dalam fragment tersebut tanpa harus membuat ulang.


## Lifecycle Fragment
> Pada dasarnya Fragment merupakan salah satu komponen pada Android Studio dengan fungsi yang hampir sama seperti activity tetapi memiliki “lifecycle” yang berbeda. Berikut adalah lifecycle dalam Fragment:
- **onAttach()** dipanggil saat sebuah fragment terhubung ke activity.
- **onCreate()** diapnggil saat sebuah fragment dibuat (objeknya di memori).
- **onCreateView()** dipanggil saat fragment sudah siap membaca sebuah layout.
- **onViewCreated()** dipanggil setelah onCreateView() dan memastikan layout yang dibaca fragment adalah non-null. Semua pengaturan view seperti pembacaan findViewById, menambah onClickListener dapat dilakukan di sini.
- **onActivityCreated()** dipanggil setelah activity pembaca sudah menyelesaikan onCreate()-nya.
- **onStart()** dipanggil setelah fragment siap untuk ditampilkan di layar.
- **onResume()** Dipakai untuk melakukan pembacaan data yang lebih “rumit” seperti lokasi, sensor, dll.
- **onPause()** Tempat melepas data “rumit”. Lakukan commit di sini.
- **onDestroyView()** dipanggil saat layout sebuah fragment akan dihapus dari memori, namun fragmentnya masih ada di memori.
- **onDestroy()** dipanggil jika fragment sudah tidak dipakai.
- **onDetach()** dipanggil saat fragment tidak lagi terhubung ke sebuah activity.

### Hasil Program
![ezgif-2-c7e90efbf27c](https://user-images.githubusercontent.com/60590053/109190828-1a19e000-77c8-11eb-90a0-54d6dd5452d7.gif)

- Fragment 1 : Halaman Hewan Kucing

![WhatsApp Image 2021-02-25 at 22 27 23 (2)](https://user-images.githubusercontent.com/60590053/109190846-1dad6700-77c8-11eb-9c52-e0664bf2baa9.jpeg)

- Fragment 2 : Halaman Hewan Anjing

![WhatsApp Image 2021-02-25 at 22 26 16](https://user-images.githubusercontent.com/60590053/109190853-200fc100-77c8-11eb-9d13-790c4b119c26.jpeg)

## Terimakasih
