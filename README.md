PERTANYAAN PRAKTIKUM SEQUENTIAL SEACRH
1. Jelaskan perbedaan metod tampilDataSearch dan tampilPosisi pada class
MahasiswaBerprestasi!
jawaban: tampildataSearch untuk menampilkan data yang telah disimpan
jika tampilPosisi untuk menampilkan posisi index yang ditemukan

2. Jelaskan fungsi break pada kode program di bawah ini!
if (listMhs[j].ipk == cari){
    posisi=j;
    break;
}
jawaban : untuk menghentikan perulangan Loop saat data sudah ditemukan

3. Apa fungsi variabel pos atau indeks hasil pencarian dalam program sequential search?
jawaban : pos digunakann untuk menyimpan posisi index data yang ditemukan, menunjukkan letka data dalam  array

4. Jika terdapat lebih dari satu data dengan nilai yang sama, hasil pencarian sequential search yang dibuat di atas akan menampilkan data ke berapa? Jelaskan.
jawabann: data yang pertama kali temukan, karena adanya break jadi loop berhenti di penemuan pertama

dibuat di atas akan menampilkan data ke berapa? Jelaskan.
5. Berkaitan dengan pertanyaan nomor 2 di atas, apa yang terjadi jika perintah break dihapus dari
kode di atas?
jawaban : program akan terus mencari sampai akhir array


PERTANYAAN PRAKTIKUM BINARY SEARCH
1.	Tunjukkan pada kode program yang mana proses divide dijalankan!
jawaban : pada mid = (left+right)/2;

2.	Tunjukkan pada kode program yang mana proses conquer dijalankan!
jawaban : if (cari == listMhs[mid].ipk){
    return mid;
}
else if (listMhs[mid].ipk > cari){
    return findBinarySearch(cari, left, mid - 1);
}
else {
    return findBinarySearch(cari, mid + 1, right);
}

3.	Apa fungsi left, right, dan mid?
jawaban : 
left = batas kiri area pencarian
right = batas kanan area pencarian
mid = index tengah yang digunakan untuk membandingkan data

4.	Jika data IPK yang dimasukkan tidak urut. Apakah program masih dapat berjalan? Mengapa demikian?
jawaban : Program tetap dapat dijalankan, tetapi hasil pencarian bisa tidak akurat atau salah.

5.	Jika IPK yang dimasukkan dari IPK terbesar ke terkecil (misal: 3.8, 3.7, 3.5, 3.4, 3.2) dan elemen yang dicari adalah 3.2. Bagaimana hasil dari binary search? Apakah sesuai? Jika tidak sesuai maka ubahlah kode program binary seach agar hasilnya sesuai?
jawaban : sudah di modif 

6.	Jelaskan bagaimana binary search menentukan bahwa data yang dicari tidak ditemukan di dalam array.
jawaban : Jika batas kiri sudah melewati batas kanan, berarti seluruh data sudah dicek dan data tidak ditemukan.

7.	Modifikasi program di atas yang mana jumlah mahasiswa yang diinputkan sesuai dengan masukan dari keyboard.
jawaban : sudah di modiff
