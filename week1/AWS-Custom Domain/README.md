# Dumbways Bootcamp DevOps
## Week 1
### AWS-Custom Domain


1. Buka dashboard cloudflare, lalu klik DNS, dan Add Route
   
   ![1]()

2. Isi DNS management, Name disesuaikan, IPv4 menggunakan IP Publik dari Public Instance

   ![2]()

3. Lalu buka konfigurasi reverse proxy.

    ![3]()

4. Ubah server_name dengan domain yang baru sama dibuat.
   
   ![4]()

5. Restart service nginx
   
   ![5]()

6. Akses project dengan memasukan domain baru pada browser.

    ![6]()