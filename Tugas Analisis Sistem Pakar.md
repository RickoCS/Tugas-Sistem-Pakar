# Aplikasi Berbasis Mobile untuk Pencarian Rute Angkutan Umum Kota Menggunakan Algoritma Depth First Search

Tujuan dari dibuatnya sistem ini adalah untuk memberikan kemudahan kepada masyarakat pengguna angkutan umum dalam mencari informasi kode angkutan umum dan mendapatkan solusi rute angkutan umum yang tepat dan terdekat. 
Sistem Pakar terbagi menjadi 3 bagian penting yaitu User Interface, Mesin Interference dan Knowledge Base. Berikut merupakan penjelasan mengenai 3 bagian penting tersebut. <br />

**User Interface** <br />

User interface yang digunakan dalam sistem pakar ini yaitu dengan adanya kode angkutan Antarmuka pengguna dalam sistem pakar ini didesain dengan menggunakan beberapa elemen kunci, 
seperti kode angkutan umum, formulir untuk menetapkan tujuan, daftar rute transportasi umum, dan tampilan peta melalui Google Maps. Formulir untuk menetapkan tujuan mencakup kolom teks, spinner untuk alamat, 
dan tombol pencarian untuk memudahkan pengguna dalam menyebutkan tujuan mereka. Daftar rute transportasi umum menampilkan kode rute, dan pengguna dapat melihat jalur transportasi umum tersebut melalui integrasi dengan Google Maps. <br />
Arsitektur aplikasi ini melibatkan serangkaian langkah yang intuitif bagi pengguna. Pengguna diminta untuk menetapkan tujuan dengan mengisi formulir dan mengklik tombol pencarian. 
Setelahnya, sistem menampilkan daftar rute transportasi umum yang relevan. Pengguna dapat memilih rute yang diinginkan, dan sistem akan menampilkan rute tersebut secara visual di peta Google Maps. 
Penggunaan GPS memastikan akurasi lokasi pengguna, sementara formula di dalam sistem diimplementasikan untuk menghitung jarak antara koordinat pengguna dan koordinat rute transportasi umum terpilih. <br />
Antarmuka pengguna secara khusus memanfaatkan fragmen peta dari Google Maps V2 untuk menyajikan rute transportasi umum dengan jelas. Diagram aktivitas aplikasi memberikan gambaran lebih lanjut tentang alur kerja aplikasi, 
termasuk proses pencarian alamat tujuan, perbandingan jarak antara posisi pengguna dan koordinat rute yang terhubung, dan pengelolaan serta penyajian rute sebagai daftar yang mudah dipahami oleh pengguna. Dengan demikian, 
sistem ini dirancang untuk memberikan pengalaman pengguna yang terpadu dan efisien dalam merencanakan perjalanan dengan transportasi umum. <br />
 
**Mesin Interference**<br />

Algoritma Depth First Search (DFS) yang digunakan dalam sistem pakar ini  adalah untuk melakukan penelusuran pada graf atau pohon yang dimulai dari simpul akar (root) dan mengeksplorasi sejauh mungkin sepanjang setiap cabang sebelum mundur. 
Pada setiap simpul, algoritma DFS akan mengunjungi anak simpul pertama yang bertetangga dengan simpul akar dan melanjutkan penelusuran ke tingkat terdalamnya sebelum kembali ke simpul lain yang juga bertetangga dengan simpul akar.<br />
Dalam konteks sistem pakar ini setiap simpul mewakili tempat tujuan dari rute angkutan umum yang sudah tersedia pada aplikasi pencarian rute angkutan umum. 
Algoritma DFS digunakan untuk mencari rute terpendek antara posisi pengguna aplikasi dan beberapa pilihan rute yang tersedia. 
Algoritma ini akan mencari atau mengunjungi anak simpul dari suatu simpul sebelum mengunjungi simpul tetangganya. DFS akan terus melintasi atau mencari jalur 
sampai menemukan solusi atau mencapai simpul terakhir. <br />
Pemilihan algoritma DFS sebagai alat bantu dalam pencarian rute angkutan umum adalah karena algoritma DFS membutuhkan 
penggunaan memori yang efisien karena hanya simpul-simpul pada jalur yang aktif yang disimpan. Selain itu, jika solusi yang dicari berada pada level yang dalam dan paling kiri, algoritma DFS akan menemukannya dengan cepat.
Dalam implementasinya pada aplikasi, algoritma DFS digunakan untuk mencari rute terdekat dari posisi pengguna aplikasi dengan menggunakan data koordinat dan jarak antara titik awal dan titik tujuan. Data koordinat tersebut kemudian dicocokan dengan data rute angkutan umum yang tersedia dan algoritma DFS akan bekerja untuk mencari rute terdekat menuju titik tujuan. Hasil pencarian rute menggunakan algoritma DFS ini kemudian ditampilkan kepada pengguna dengan bantuan peta yang disediakan Google Maps. <br />

**Knowledge Base**<br />

Knowledge base adalah kumpulan informasi, pengetahuan, dan fakta yang disimpan dalam sistem pakar atau sistem lainnya. Knowledge base berfungsi sebagai basis data yang berisi aturan-aturan, heuristik, fakta-fakta, dan pengetahuan lainnya yang digunakan oleh sistem untuk melakukan penalaran dan memberikan solusi atau rekomendasi. <br />
Knowledge base merupakan komponen penting dalam sistem pakar karena berperan dalam penyimpanan dan pengelolaan pengetahuan yang diperlukan oleh sistem. Dalam knowledge base, pengetahuan dapat direpresentasikan dalam berbagai bentuk, seperti aturan-aturan berbasis IF-THEN, basis data, pohon keputusan, atau model matematika. Knowledge base dapat diperbarui dan diperluas seiring waktu dengan penambahan pengetahuan baru atau revisi terhadap pengetahuan yang ada. Hal ini memungkinkan sistem pakar untuk terus berkembang dan meningkatkan kualitas penalaran serta hasil yang diberikan. Penting untuk menjaga keakuratan dan kekonsistenan knowledge base agar sistem pakar dapat memberikan hasil yang dapat diandalkan. Pemeliharaan dan pembaruan knowledge base secara teratur sangat penting untuk menjaga relevansi dan performa sistem pakar.<br />
Jadi, knowledge base adalah kumpulan informasi dan pengetahuan yang digunakan oleh sistem pakar atau sistem lainnya untuk melakukan penalaran dan memberikan solusi atau rekomendasi.<br />