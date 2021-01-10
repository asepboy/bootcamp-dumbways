# Dumbways Bootcamp DevOps
## Week 4
### Setup Monitoring Server

Pada Server Monitoring akan diinstall 3 buah aplikasi pendukung, yaitu Node Exporter, Prometheus, dan Grafana.
    Pada kegiatan ini saya akan menerapkan monitoring dengan 1 master dan 1 slave, hanya untuk melihat trend apakah monitoring dapat dilakukan atau tidak.

### Node Exporter
Node exporter akan diinstall disemua server yang bersangkutan.
1. Melakukan Update pada semua server yang bersangkutan.
   
    ![1](/week4/SetupMonitoringServer/img/Node%20Exporter/1.png)

    ![8](/week4/SetupMonitoringServer/img/Node%20Exporter/8.png)

2. Mendownload file node exporter
   
   ![2](/week4/SetupMonitoringServer/img/Node%20Exporter/2.png)

   ![9](/week4/SetupMonitoringServer/img/Node%20Exporter/9.png)

3. Lalu mengextract file yang sudah didownload tadi
   
   ![3](/week4/SetupMonitoringServer/img/Node%20Exporter/3.png)

   ![10](/week4/SetupMonitoringServer/img/Node%20Exporter/10.png)

4. Pindahkan file hasil extract ke /usr/local/bin
   
   ![4](/week4/SetupMonitoringServer/img/Node%20Exporter/4.png)

   ![11](/week4/SetupMonitoringServer/img/Node%20Exporter/11.png)

5. Tambahkan user untuk node_exporter
   
   ![5](/week4/SetupMonitoringServer/img/Node%20Exporter/5.png)

   ![12](/week4/SetupMonitoringServer/img/Node%20Exporter/12.png)

6. Lalu buat file node_exporter.service di /etc/systemd/system/
   
   ![6](/week4/SetupMonitoringServer/img/Node%20Exporter/6.png)

   ![13](/week4/SetupMonitoringServer/img/Node%20Exporter/13.png)

7. Selanjutnya jalankan service node_exporter
   
   ![7](/week4/SetupMonitoringServer/img/Node%20Exporter/7.png)

   ![14](/week4/SetupMonitoringServer/img/Node%20Exporter/14.png)

8. Melakukan test akses ke node exporter dengan curl
   
   ![15](/week4/SetupMonitoringServer/img/Node%20Exporter/15.png)


### Prometheus
    Prometheus akan diinstall hanya pada server master.

1. Mendownload file node exporter
   
   ![1](/week4/SetupMonitoringServer/img/Prometheus/1.png)

2. Lalu mengextract file yang sudah didownload tadi
   
   ![2](/week4/SetupMonitoringServer/img/Prometheus/2.png)

3. Pindahkan file hasil extract ke /usr/local/bin
   
   ![3](/week4/SetupMonitoringServer/img/Prometheus/3.png)

4. Lalu buat folder prometheus pada /etc/ dan pada /var/lib/

    ![4](/week4/SetupMonitoringServer/img/Prometheus/4.png)

5. Setelah itu pindahkan folder /console_libraries/ yang ada di folder hasil ekstraksi ke /etc/prometheus/

    ![5](/week4/SetupMonitoringServer/img/Prometheus/5.png)

6. Selanjutnya membuat file configurasi prometheus, dengan nama prometheus.yml, dan memberikan detail job yang akan dilakukan, dana server mana saja yang akan di monitor.
   
    ![6](/week4/SetupMonitoringServer/img/Prometheus/6.png)

7. Tambahkan user untuk prometheus

    ![7](/week4/SetupMonitoringServer/img/Prometheus/7.png)

8. Lalu ubah kepemilikan folder /etc/prometheus dan /var/lib/prometheus ke user prometheus
   
    ![8](/week4/SetupMonitoringServer/img/Prometheus/8.png)

9. Lalu tambahkan file prometheus.service di /etc/systemd/system/, dengan isinya sebagai berikut.
    
    ![9](/week4/SetupMonitoringServer/img/Prometheus/9.png)

10. Jalankan service prometheus
    
    ![10](/week4/SetupMonitoringServer/img/Prometheus/10.png)

11. Melakukan test akses ke prometheus dengan curl
    
    ![11](/week4/SetupMonitoringServer/img/Prometheus/11.png)

### Grafana
Prometheus akan diinstall hanya pada server master.
1. Download gpg.key untuk package grafana, dan tambahkan ke apt
   
    ![1](/week4/SetupMonitoringServer/img/Grafana/1.png)

2. Tambahkan repository grafana
   
    ![2](/week4/SetupMonitoringServer/img/Grafana/2.png)

3. Update lalu install grafana
   
   ![3](/week4/SetupMonitoringServer/img/Grafana/3.png)

4. Jalankan service grafana
   
   ![4](/week4/SetupMonitoringServer/img/Grafana/4.png)

5. Lalu pada config file grafana (/etc/grafana/grafana.ini), allow_sign_up dan auth.anonymous dibuat false.

    ![5](/week4/SetupMonitoringServer/img/Grafana/5.png)

    ![6](/week4/SetupMonitoringServer/img/Grafana/6.png)

6. Restart service grafana
   
   ![7](/week4/SetupMonitoringServer/img/Grafana/7.png)

7. Lakukan pengetesan dengan menggunakan curl

    ![8](/week4/SetupMonitoringServer/img/Grafana/8.png)


### Reverse Proxy, Domain, SSL
1. Buat rules reverse proxy untuk grafana di /etc/nginx/, lalu tambahkan direktori rules baru ke file config nginx. Setelah itu restart service nginx dan akses menggunakan browser dengan menggunakan IP Public Server.

    ![1](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/1.png)

    ![2](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/2.png)

    ![3](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/3.png)

2. Daftarkan domain yang telah ditentukan di cloudflare, lalu ubah server_name pada rules yang sudah dibuat dengan domain baru. Setelah itu restart service nginx dan akses domain baru dengan menggunakan browser.
   
   ![4](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/4.png)

   ![5](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/5.png)

   ![6](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/6.png)

3. Buat SSL configuration dengan perintah berikut, dan pastikan domain berhasil didaftarkan. Akses domain baru dengan menggunakan browser.

    ![7](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/7.png)

    ![8](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/8.png)

    ![9](/week4/SetupMonitoringServer/img/ReverseProxyCustomDomain&SSL/9.png)


### Authentication Prometheus
    Tahap ini maksudkan agar ketika mengakses prometheus menggunakan browser, ada authentikasi terlebih dahulu. Dan pastikan buat reverse proxy terlebih dahulu, agar dapat diakses menggunakan browser.

1. Install apache2-utils. Apache2-utils dapat membantu untuk membuat password dan user.

   ![1](/week4/SetupMonitoringServer/img/authPrometheus/1.png)
 
2. Buat direktori baru untuk menyimpan file configurasi auth, dan jalankan perintah htpasswd untuk membuat password untuk user admin. user dapat disesuaikan. Lalu akan diminta untuk memasukan password untuk user admin.
   
    ![2](/week4/SetupMonitoringServer/img/authPrometheus/2.png)

3. Lalu pada rules reverse proxy, tambahkan line seperti dibawah agar dapat membaca file authentikasi yang baru dibuat. 
   
   ![3](/week4/SetupMonitoringServer/img/authPrometheus/3.png)

4. Lalu akses menggunakan browser, dan akan muncul pop-up authentikasi seperti dibawah.
   
   ![4](/week4/SetupMonitoringServer/img/authPrometheus/4.png)

   ![5](/week4/SetupMonitoringServer/img/authPrometheus/5.png)