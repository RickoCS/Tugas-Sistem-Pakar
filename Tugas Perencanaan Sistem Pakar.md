# Sistem Pakar Untuk Rekomendasi Pemilihan Tempat Wisata Dengan Menggunakan Fordward Chaining

Latar belakang dibuatnya sistem pakar ini adalah untuk mempermudah dan meningkatkan efisiensi dalam pemilihan obyek wisata bagi para wisatawan. Saat ini, pemilihan obyek wisata dilakukan dengan cara langsung mendatangi travel agency, 
namun seringkali hasilnya tidak sesuai dengan harapan dan biayanya pun tidak murah. Oleh karena itu, sistem pakar ini dikembangkan dengan tujuan agar wisatawan dapat merencanakan perjalanan wisata sesuai dengan keinginan dan kebutuhan mereka sendiri. 
Sistem pakar ini menggunakan pengetahuan dari agen wisata dan pakar dalam bidang pariwisata untuk memberikan rekomendasi obyek wisata yang sesuai dengan kriteria wisatawan. Dengan adanya sistem pakar ini, 
diharapkan dapat mengurangi masalah dalam pemilihan obyek wisata dan meningkatkan kepuasan wisatawan. <br />

**User Interface** <br />
Pada sistem pakar ini akan digunakan user interface atau antarmuka pengguna untuk memberikan Informasi mengenai bebeapa destinasi wisata yang ada pada kota tersebut. Pada antarmuka pengguna ini pengguna akan diberikan beberapa kriteria yang disediakan pada 
halaman utama website tersebut. Beberapa kriteria yang dapat dipilih oleh pengguna adalah jenis wisata yang diinginkan seperti wisata budaya, alam, hiburan dan rekreasi, pendidikan, belanja, dan cagar budaya. Kemudian pengguna dapat memilih biaya wisata yang diinginkan, 
biaya wisata ini berkaitan dengan biaya masuk dari tempat wisata tersebut dan juga biaya transportasi umum yang dibutuhkan untuk perjalanan menuju tempat wisata tersebut.<br />  

Setelah pengguna memasukan beberapa kriteria yang tersedia pada halaman utama tersebut, maka sistem pakar ini akan mengolah data kriteria tersebut untuk didapatkan hasil rekomendasi tempat wisata yang sesuai dengan kriteria yang dipilih. 
Kemudian pengguna dapat memilih beberapa hasil rekomendasi tempat wisata yang sudah diberikan. Apabila pengguna sudah memilih tempat wisata yang merupakan hasil rekomendasi tempat wisata ini, maka pengguna akan dialihkan menuju Google Maps untuk ditampilkan 
rute menuju tempat wisata tersebut dari titik koordinat pengguna. Pada Google Maps tersebut akan diberikan informasi mengenai jarak tempuh dan perkiraan waktu perjalanan menuju tempat wisata tersebut.<br />    
 
**Mesin Interferance**<br />
Metode inferensi yang digunakan dalam  perencanaa sistem pakar ini adalah forward chaining. Forward chaining adalah strategi inferensi yang digunakan dalam sistem pakar berbasis aturan. 
Dalam strategi ini, sistem pakar akan menelusuri pohon inferensi yang dikembangkan dengan model pohon keputusan.  Pohon keputusan tersebut berisikan data masukan berupa kriteria-kriteria menuju pada konklusi, yaitu obyek wisata yang dicari.<br />

Dalam sistem pakar E-Tourism, aturan-aturan produksi yang menghubungkan kriteria dengan obyek wisata disimpan dalam basis pengetahuan. Ketika pengguna memasukkan kriteria wisata yang diinginkan, 
sistem pakar akan mencocokkan kriteria tersebut dengan aturan-aturan yang ada dalam basis pengetahuan. Jika terdapat aturan yang sesuai dengan kriteria yang dimasukkan, 
maka sistem pakar akan menyimpulkan bahwa obyek wisata yang sesuai dengan aturan tersebut juga sesuai dengan kriteria pengguna.<br />

Proses forward chaining berlanjut dengan mencari aturan-aturan lain yang dapat diterapkan berdasarkan konklusi-konklusi yang telah diperoleh sebelumnya. Hal ini dilakukan secara berulang hingga tidak ada lagi aturan yang dapat 
diterapkan atau hingga mencapai konklusi akhir, yaitu rekomendasi obyek wisata yang sesuai dengan kriteria pengguna.
Dengan menggunakan strategi forward chaining, sistem pakar dapat memberikan rekomendasi obyek wisata yang sesuai dengan preferensi dan kebutuhan pengguna berdasarkan aturan-aturan yang ada dalam basis pengetahuan.<br />

**Knowledge Base**<br />
Sistem pakar ini membutuhkan suatu data untuk digunakan sebagai basis pengetahuan sistem pakar tersebut. Data yang digunakan sebagai basis pengetahuan dari sistem pakar ini adalah sebagai berikut:<br /> 

1. Data mengenai jenis-jenis wisata, seperti wisata budaya, alam, hiburan dan rekreasi, pendidikan, belanja, dan cagar budaya.<br />
2. Data mengenai karakteristik masing-masing obyek wisata, termasuk nama obyek wisata, keterangan, dan kriteria yang relevan.<br />
3. Data mengenai rekomendasi untuk masing-masing obyek wisata berdasarkan kriteria yang ditentukan.<br />
4. Data mengenai informasi spesifik tentang suatu obyek wisata, seperti fasilitas, lokasi, dan aktivitas yang tersedia.<br />
5. Data mengenai budget atau perkiraan biaya yang dibutuhkan selama perjalanan wisata.<br />

Data tersebut diperoleh melalui akuisisi pengetahuan dari berbagai sumber, seperti buku-buku yang relevan, internet, dan wawancara dengan pakar pariwisata. Pengetahuan ini kemudian disimpan dalam sistem pakar dalam bentuk aturan produksi 
IF-THEN yang menghubungkan kriteria dengan obyek wisata dan rekomendasinya.<br />
