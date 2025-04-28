Tugas 6 Organisasi Arsitektur Komputer
# Multiprosesor Simetris dan Tidak Simetris
![AMD Ryzen](https://github.com/user-attachments/assets/51170df1-4772-45dc-a812-b540efcb9ee2)
Multiprosesor Simetri adalah Semua prosesor punya hak akses yang sama ke memori, ke sistem operasi, dan ke I/O (input/output).
Setiap prosesor bisa menjalankan semua tugas yang ada. Tidak ada pembagian "bos" dan "anak buah" antar CPU.
## ciri-ciri:
1. Semua CPU berbagi memori utama (RAM).
2. Setiap CPU bisa mengakses semua perangkat keras.
3. Beban kerja bisa dibagi rata (load balancing lebih mudah).
4. Kalau satu CPU rusak, sistem bisa tetap jalan dengan CPU lain (lebih tahan gangguan).
5. Umumnya dipakai di server modern, workstation, dan komputer multi-core.

![image](https://github.com/user-attachments/assets/0665d4ae-c87d-496f-8108-915df9fe64d2)
Multiprosesor tidak simetris adalah multiprosesor dengan pembagian tugas khusus antar CPU. Biasanya satu prosesor utama (master) yang ngatur, dan prosesor lain (slave) hanya menjalankan perintah.
## ciri-ciri
1. CPU master bertanggung jawab untuk mengelola sistem operasi dan pembagian tugas.
2. CPU slave hanya menjalankan tugas tertentu yang diperintahkan master.
3. Efisien untuk sistem yang tugasnya spesifik atau real-time.
4. Sistemnya lebih sederhana, tapi kalau CPU master gagal, seluruh sistem bisa berhenti.
5. Umumnya dipakai di sistem embedded, robotik, smartphone, konsol game.

## Kesimpulan:
  Multiprosesor merupakan teknologi penting dalam dunia komputasi modern, di mana lebih dari satu prosesor bekerja bersama untuk meningkatkan kinerja sistem. Berdasarkan cara kerja dan pembagian tugasnya, multiprosesor dibagi menjadi dua jenis utama, yaitu Multiprosesor Simetris (SMP) dan Multiprosesor Tidak Simetris (AMP).

  Pada sistem Multiprosesor Simetris (SMP), semua prosesor memiliki kedudukan yang setara dan dapat menjalankan tugas secara bersamaan, berbagi akses ke memori, perangkat keras, serta sistem operasi. Hal ini memungkinkan pembagian beban kerja secara seimbang, meningkatkan kecepatan pemrosesan, dan memperkuat ketahanan sistem terhadap kegagalan salah satu prosesor. SMP banyak digunakan dalam komputer multi-core, server, dan workstation modern yang membutuhkan performa tinggi dan fleksibilitas dalam pengelolaan tugas.

  Sementara itu, pada sistem Multiprosesor Tidak Simetris (AMP), terdapat pembagian peran antara prosesor utama (master) dan prosesor pembantu (slave). Prosesor master mengatur seluruh jalannya sistem, sedangkan prosesor slave bertugas menjalankan tugas-tugas tertentu sesuai arahan. Pendekatan ini cocok untuk sistem-sistem yang membutuhkan efisiensi khusus, seperti smartphone, robot industri, router jaringan, dan perangkat embedded lainnya. AMP menawarkan keunggulan dalam kesederhanaan desain dan penghematan sumber daya, meskipun biasanya kurang fleksibel dibandingkan SMP.

  Secara keseluruhan, baik sistem SMP maupun AMP memiliki keunggulan masing-masing tergantung pada kebutuhan penggunaannya. SMP lebih cocok untuk sistem yang membutuhkan fleksibilitas tinggi dan pembagian kerja kompleks, sementara AMP lebih efektif untuk aplikasi yang memerlukan pengaturan tugas secara spesifik dan efisiensi sumber daya. Pemilihan jenis multiprosesor yang tepat akan sangat berpengaruh terhadap kinerja, keandalan, dan efektivitas sistem yang dibangun.
