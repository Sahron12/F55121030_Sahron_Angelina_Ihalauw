# Nama : Sahron Angelina Ihalauw
# NIM  : F 551 21 030
# Kelas: A 
# Matakuliah PAA

# 1. Bubble dan Insertion
- Worst case:
Bubble Sort: Pada worst case, Bubble Sort memiliki kompleksitas waktu O(n^2), di mana n adalah jumlah elemen dalam list yang diurutkan. Worst case terjadi ketika elemen-elemen dalam list terurut secara terbalik. Dalam implementasi ini, Bubble Sort akan melakukan iterasi sebanyak n-1 kali untuk memindahkan elemen-elemen terbesar ke posisi yang benar pada setiap iterasi.
Insertion Sort: Pada worst case, Insertion Sort juga memiliki kompleksitas waktu O(n^2). Worst case terjadi ketika elemen-elemen dalam list terurut secara terbalik. Dalam implementasi ini, Insertion Sort akan melakukan iterasi sebanyak n-1 kali untuk memindahkan setiap elemen ke posisi yang benar pada setiap iterasi.

- Best case:
Bubble Sort: Pada best case, Bubble Sort memiliki kompleksitas waktu O(n), di mana n adalah jumlah elemen dalam list yang diurutkan. Best case terjadi ketika list sudah terurut secara ascending. Dalam implementasi ini, Bubble Sort akan melakukan iterasi sebanyak n-1 kali pada iterasi pertama dan tidak ada perubahan pada iterasi selanjutnya karena list sudah terurut.
Insertion Sort: Pada best case, Insertion Sort memiliki kompleksitas waktu O(n), di mana n adalah jumlah elemen dalam list yang diurutkan. Best case terjadi ketika list sudah terurut secara ascending. Dalam implementasi ini, Insertion Sort akan melakukan iterasi sebanyak n-1 kali pada iterasi pertama dan tidak ada perubahan pada iterasi selanjutnya karena list sudah terurut.

- Average case:
Bubble Sort: Pada average case, Bubble Sort memiliki kompleksitas waktu O(n^2), di mana n adalah jumlah elemen dalam list yang diurutkan. Average case terjadi ketika elemen-elemen dalam list tidak terurut secara terbalik atau sudah terurut sebagian. Dalam implementasi ini, Bubble Sort akan melakukan iterasi sebanyak n-1 kali pada setiap iterasi dan memindahkan elemen-elemen yang tidak terurut ke posisi yang benar.
Insertion Sort: Pada average case, Insertion Sort memiliki kompleksitas waktu O(n^2), di mana n adalah jumlah elemen dalam list yang diurutkan. Average case terjadi ketika elemen-elemen dalam list tidak terurut secara terbalik atau sudah terurut sebagian. Dalam implementasi ini, Insertion Sort akan melakukan iterasi sebanyak n-1 kali pada setiap iterasi dan memindahkan elemen-elemen yang tidak terurut ke posisi yang benar.

# 2. TSP dan Djikstra
- Algoritma TSP:
Algoritma ini digunakan untuk mencari jalur terpendek yang melalui semua kota (dimulai dan berakhir di kota yang sama).
Algoritma menggunakan pendekatan rekursif dengan backtracking menggunakan Depth-First Search (DFS).
Selama rekursi, algoritma membangun jalur dan menghitung biaya minimum.
Jika semua kota telah dikunjungi dan kembali ke kota awal, algoritma memperbarui biaya minimum jika ditemukan jalur yang lebih pendek.
Pada akhirnya, algoritma mengembalikan biaya minimum dan waktu eksekusi.

- Algoritma Dijkstra:
Algoritma ini digunakan untuk mencari jalur terpendek dari satu titik awal ke semua titik lain dalam grafik.
Algoritma menggunakan pendekatan Greedy dengan menggunakan Priority Queue (heapq) untuk memilih jalur dengan jarak terpendek pada setiap langkah.
Algoritma memperbarui jarak minimum ke setiap titik saat menjelajahi grafik.
Pada akhirnya, algoritma mengembalikan daftar jarak terpendek dari titik awal ke semua titik lain dan waktu eksekusi.

- Fungsi print_path(path):
Fungsi ini digunakan untuk mencetak jalur dalam format yang lebih mudah dibaca.

- Fungsi main():
Fungsi ini berfungsi sebagai titik masuk program.
Grafik didefinisikan di dalam fungsi ini.
Pengguna diminta untuk memilih algoritma (TSP atau Dijkstra).
Hasil akhir, termasuk jalur terpendek dan waktu eksekusi, dicetak berdasarkan pilihan pengguna.

- Analisis Algorithm:
Worst case untuk TSP dan Dijkstra adalah O(n!), di mana n adalah jumlah kota atau titik dalam grafik. Karena algoritma menggunakan pendekatan eksponensial, waktu eksekusi dapat meningkat secara drastis dengan meningkatnya jumlah kota.
Best case untuk TSP dan Dijkstra adalah O(n^2 log n), di mana n adalah jumlah kota atau titik dalam grafik. Best case terjadi ketika grafik sangat jarang dan terdapat sedikit edge yang perlu diperiksa.
Average case untuk TSP dan Dijkstra juga berkisar O(n^2 log n), tetapi ini dapat bervariasi tergantung pada struktur grafik dan jalur yang dipilih.
