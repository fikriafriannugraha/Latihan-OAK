# Latihan-OAK

### **1. Struktur Antar Hubungan dan Contohnya**  
Struktur antar hubungan adalah pola atau cara elemen-elemen dalam suatu sistem saling berinteraksi dan berhubungan satu sama lain. Struktur ini bisa ditemukan dalam berbagai bidang, seperti organisasi, jaringan komputer, ekonomi, dan sosial.

#### **Contoh Struktur Antar Hubungan:**  
- **Hierarkis** → Struktur organisasi perusahaan (CEO → Manajer → Karyawan).  
- **Jaringan (Network)** → Jaringan komputer (server-client).  
- **Linear (Rantai)** → Rantai pasokan (Supplier → Produsen → Distributor → Konsumen).  
- **Fungsional** → Departemen dalam perusahaan (Keuangan, Pemasaran, Produksi).  
- **Timbal Balik (Reciprocal)** → Hubungan diplomasi antar negara.  

---

### **2. Penyebab Penurunan Kinerja Saat Terlalu Banyak Modul/Perangkat Terhubung ke Bus**  
Ketika terlalu banyak modul atau perangkat dihubungkan pada bus, maka terjadi penurunan kinerja yang disebabkan oleh:  

1. **Kontensi Bus (Bus Contention):**  
   - Banyak perangkat bersaing untuk menggunakan bus, sehingga terjadi antrian dan waktu akses meningkat.  

2. **Lalu Lintas Data Tinggi (Traffic Congestion):**  
   - Meningkatnya jumlah perangkat meningkatkan jumlah data yang dikirim, menyebabkan bottleneck.  

3. **Waktu Propagasi Bertambah:**  
   - Semakin panjang jalur bus, semakin lama waktu yang dibutuhkan sinyal untuk mencapai tujuan.  

4. **Delay Akses Memori:**  
   - Jika banyak perangkat mencoba mengakses memori secara bersamaan, waktu respons memori meningkat.  

5. **Kapasitas Bandwidth Terbatas:**  
   - Bus memiliki bandwidth terbatas, sehingga kelebihan beban menyebabkan penurunan kecepatan transfer data.  

---

### **3. Alasan Perangkat Berprioritas 16 Memiliki Waktu Tunggu Rata-Rata Paling Rendah**  
Dalam sistem dengan **Skema Prioritas Berjenjang**, perangkat dengan prioritas lebih rendah sering mendapatkan akses lebih cepat karena:  

1. **Mekanisme Preemption (Penggantian Cepat):**  
   - Perangkat berprioritas tinggi mungkin sering ditunda oleh proses-proses penting lainnya, sementara perangkat dengan prioritas rendah sering dieksekusi lebih cepat karena tidak bersaing dengan tugas-tugas kritis.  

2. **Distribusi Permintaan:**  
   - Jika perangkat berprioritas tinggi menangani proses yang lebih kompleks, waktu eksekusinya lebih lama dibanding perangkat berprioritas lebih rendah yang sering hanya membutuhkan sedikit sumber daya dan dapat segera dieksekusi.  

---

### **4. Kondisi di Mana Aturan Ini Tidak Berlaku**  
Aturan bahwa perangkat dengan prioritas rendah memiliki waktu tunggu rata-rata paling rendah tidak berlaku dalam kondisi berikut:  

1. **Sistem Beban Tinggi (High Load System):**  
   - Jika terlalu banyak tugas dengan prioritas tinggi yang menumpuk, perangkat prioritas rendah bisa mengalami starvation (kelaparan sumber daya) dan tidak mendapatkan eksekusi dalam waktu lama.  

2. **Sistem Dengan Preemptive Scheduling:**  
   - Jika sistem menggunakan preemptive scheduling yang selalu mendahulukan tugas prioritas tinggi, maka perangkat prioritas rendah akan sering tertunda.  

3. **Bursty Workload (Beban Kerja Lonjakan Tinggi):**  
   - Jika tiba-tiba ada lonjakan proses dengan prioritas tinggi yang masuk dalam waktu bersamaan, maka perangkat prioritas rendah akan mengalami delay lebih lama.  

4. **Algoritma Penjadwalan Tertentu (Round Robin atau FIFO):**  
   - Jika sistem menggunakan algoritma seperti Round Robin atau First Come First Serve (FIFO), maka semua perangkat mendapatkan waktu eksekusi yang sama tanpa mempertimbangkan prioritas.  

---

### Sumber Yang Saya Ambil :
1. **Jurnal dan Artikel:**  
   - IEEE Xplore Digital Library (https://ieeexplore.ieee.org/)  
   - ACM Digital Library (https://dl.acm.org/)  

2. **Sumber Daring & Dokumentasi Resmi:**  
   - Documentation IBM tentang *Bus Architecture*  
   - ResearchGate dan arXiv untuk artikel terkait sistem komputer  
