# Tutorial Install Packet Tracer di Manjaro / Arch Linux
Cara Install Cisco Packet Tracer di Manjaro/Arch Linux
--
1. Download file yang saya lampirkan di repository ini (packettracer.tar.gz) 
2. Buka terminal dan arahkan ke direktori file yang sudah didownload tadi
   ```
   cd Downloads
   ```
3. Ekstrak file tersebut dengan cara :
   ```
   tar -xzvf packettracer.tar.gz
   ```
4. Download Packet Tracer untuk Ubuntu (.deb) di website Netacad (www.netacad.com)
5. Salin hasil download (file yang berekstensi .deb) tadi ke folder packettracer yang sudah kita ekstrak sebelumnya (langkah 3)
6. Buka terminal di direktori packettracer
    ```
   cd Downloads/packettracer
   ```
7. Sekarang kita buat paket dengan perintah :
   ```
   makepkg
   ```
8. Install paket dengan cara :
   ```
   makepkg -i
   ```
   atau :
   ```
   sudo pacman -U packettracer.pkg.tar.xz
   ```
9. Selesai
