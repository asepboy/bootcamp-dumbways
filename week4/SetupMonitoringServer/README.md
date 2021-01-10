# Dumbways Bootcamp DevOps
## Week 4
### Setup Monitoring Server

    Pada Server Monitoring akan diinstall 3 buah aplikasi pendukung, yaitu Node Exporter, Prometheus, dan Grafana.
    Pada kegiatan ini saya akan menerapkan monitoring dengan 1 master dan 1 slave, hanya untuk melihat trend apakah monitoring dapat dilakukan atau tidak.

### Node Exporter
    Node exporter akan diinstall disemua server yang bersangkutan.
1. Melakukan Update pada semua server yang bersangkutan.
   
    ![1]()

    ![8]()

2. Mendownload file node exporter
   
   ![2]()

   ![9]()

3. Lalu mengextract file yang sudah didownload tadi
   
   ![3]()

   ![10]()

4. Pindahkan file hasil extract ke /usr/local/bin
   
   ![4]()

   ![11]()

5. Tambahkan user untuk node_exporter
   
   ![5]()

   ![12]()

6. Lalu buat file node_exporter.service di /etc/systemd/system/
   
   ![6]()

   ![13]()

7. Selanjutnya jalankan service node_exporter
   
   ![7]()

   ![14]()

8. Melakukan test akses ke node exporter dengan curl
   
   ![15]()


### Prometheus
    Prometheus akan diinstall hanya pada server master.

1. Mendownload file node exporter
   
   ![1]()

2. Lalu mengextract file yang sudah didownload tadi
   
   ![2]()

3. Pindahkan file hasil extract ke /usr/local/bin
   
   ![3]()

4. Lalu buat folder prometheus pada /etc/ dan pada /var/lib/

    ![4]()

5. Setelah itu pindahkan folder /console_libraries/ yang ada di folder hasil ekstraksi ke /etc/prometheus/

    ![5]()

6. Selanjutnya membuat file configurasi prometheus, dengan nama prometheus.yml, dan memberikan detail job yang akan dilakukan, dana server mana saja yang akan di monitor.
   
    ![6]()

7. Tambahkan user untuk prometheus

    ![7]()

8. Lalu ubah kepemilikan folder /etc/prometheus dan /var/lib/prometheus ke user prometheus
   
    ![8]()

9. Lalu tambahkan file prometheus.service di /etc/systemd/system/, dengan isinya sebagai berikut.
    
    ![9]()

10. Jalankan service prometheus
    
    ![10]()

11. Melakukan test akses ke prometheus dengan curl
    
    ![11]()

### Grafana
    Prometheus akan diinstall hanya pada server master.
1. Download gpg.key untuk package grafana, dan tambahkan ke apt
   
    ![1]()

2. Tambahkan repository grafana
   
    ![2]()

3. Update lalu install grafana
   
   ![3]()

4. Jalankan service grafana
   
   ![4]()

5. Lalu pada config file grafana (/etc/grafana/grafana.ini), allow_sign_up dan auth.anonymous dibuat false.

    ![5]()

    ![6]()

6. Restart service grafana
   
   ![7]()

7. Lakukan pengetesan dengan menggunakan curl

    ![8]()


### Reverse Proxy, Domain, SSL
1. Buat rules reverse proxy untuk grafana di /etc/nginx/, lalu tambahkan direktori rules baru ke file config nginx. Setelah itu restart service nginx dan akses menggunakan browser dengan menggunakan IP Public Server.

    ![1]()

    ![2]()

    ![3]()

2. Daftarkan domain yang telah ditentukan di cloudflare, lalu ubah server_name pada rules yang sudah dibuat dengan domain baru. Setelah itu restart service nginx dan akses domain baru dengan menggunakan browser.
   
   ![4]()

   ![5]()

   ![6]()

3. Buat SSL configuration dengan perintah berikut, dan pastikan domain berhasil didaftarkan. Akses domain baru dengan menggunakan browser.

    ![7]()

    ![8]()

    ![9]()


### Authentication Prometheus
    Tahap ini maksudkan agar ketika mengakses prometheus menggunakan browser, ada authentikasi terlebih dahulu. Dan pastikan buat reverse proxy terlebih dahulu, agar dapat diakses menggunakan browser.

1. Install apache2-utils. Apache2-utils dapat membantu untuk membuat password dan user.

   ![1]()
 
2. Buat direktori baru untuk menyimpan file configurasi auth, dan jalankan perintah htpasswd untuk membuat password untuk user admin. user dapat disesuaikan. Lalu akan diminta untuk memasukan password untuk user admin.
   
    ![2]()

3. Lalu pada rules reverse proxy, tambahkan line seperti dibawah agar dapat membaca file authentikasi yang baru dibuat. 
   
   ![3]()

4. Lalu akses menggunakan browser, dan akan muncul pop-up authentikasi seperti dibawah.
   
   ![4]()

   ![5]()