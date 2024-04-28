# Tutorial Install Packet Tracer di Manjaro / Arch Linux**
UPDATE :
Perhatikan sha512sums di Cisco Packet Tracer yang baru (8.2.2) tapi saya malas update haha**

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
   NOTE :
   Apabila setelah langkah 7 muncul error
   
   ==> Making package: packettracer 8.2.1-1 (Sel 27 Feb 2024 09:57:02)
   
   ==> Checking runtime dependencies...
   
   ==> Missing dependencies:

     -> java-runtime>=1.7.0

     -> qt5-networkauth

     -> qt5-websockets

     -> qt5-script

   ==> Checking buildtime dependencies...

   ==> ERROR: Could not resolve all dependencies.
   
   Selesaikan dengan menginstall dependencies yang dibutuhkan dengan cara :
   ```
   sudo pacman -S jre8-openjdk qt5-networkauth qt5-websockets qt5-script
   ```

   
9. Install paket dengan cara :
   ```
   makepkg -i
   ```
   atau :
   ```
   sudo pacman -U packettracer.pkg.tar.xz
   ```
10. Selesai
