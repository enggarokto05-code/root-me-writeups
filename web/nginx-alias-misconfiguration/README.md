# Nginx-Aias Misconfiguration —Off By Slash (2024)

**Kategori:** Web

**Tingkat Kesulitan:** Medium

**Poin:** 15 Points

**Author Challenge:** .Yo0x

📝 Deskripsi Challenge
Our company's web developer has completed the development of the new intranet.
Mission: You must assess the security of this site before it goes into production.

⚡ TL;DR (Ringkasan Solusi)
1.Lakukan pengintaian (recon) menggunakan curl -v.
2.Temukan kerentanan (Directory Listing) pada bagian assets/.
3.Manfaatkan payload ../ untuk melewati sistem keamanan.

🔍 Analisis (Analysis)
1. Pengintaian Awal (Reconnaissance)
Langkah pertama yang dilakukan adalah memeriksa target:

•View Page Resource.

•Hasil temuan menarik: <!--TODO: Patch /assets/ -->

🚀 Eksploitasi (Exploitation)
Langkah Demi Langkah
Langkah 1: Menambahkan /assets pada URL untuk melihat cara server memetakan URL dan melihat respond dari server.

Langkah 2: Server menampilkan directory /assets.

🏁 FLAG:RM{4lias_M1sC0nf_HuRtS!}

💡 Pelajaran yang Diambil (Key Takeaways)

• Selalu cek apakah ada masalah atau kesalahan pada sitem konfigurasi agar tidak terjadi hal yang tidak di inginkan.

[Tips mitigasi untuk mencegah celah keamanan tersebut di dunia nyata.]
