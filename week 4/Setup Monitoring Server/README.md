# Dumbways Bootcamp DevOps Batch 4
## Week 4
### Setup Monitoring Server


1. Membuat instance di aws untuk setup monitoringnya.
2. Menginstall prometheus, grafana dan node exporter dengan menggunakan docker-compose. Maka dibuatkan file baru docker-compose.yml untuk proses instalasi monitoring dengan menggunakan docker.
    
    ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/1.png)

3. Membuat file baru untuk konfigurasi prometheus dengan node-exporter dengan nama prometheus.yml.

    ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/2.png)

4. Jalankan file docker-compose.yml dengan command "docker-compose up -d", dan lihat hasil kontainer yang berjalan.

    ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/3.png)
    
5. Mendaftarkan SSL untuk server monitoring dengan menggunakan certbot SSL dengan URL monitoring.asep.onlinecamp.id.

    ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/4.png)
    
6. Cek hasilnya apakah sudah mengimplementasikan SSL di konfigurasi nginx.

    ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/5.png)
    
7. Membuka URL monitoring.asep.onlinecamp.id dan lakukan re-password untuk masuk ke dashboard grafana.

    ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/6.png)
    
8. Mendaftarkan URL prometheus.asep.onlinecamp.id ke SSL dengan certbot, prosesnya sama dengan yang dilakukan di monitoring.asep.onlinecamp.id. Kemudian melakukan konfigurasi login untuk prometheus dengan cara menginstal terlebih dahulu apache2-utils.
  
    ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/7.png)
    
9. Membuat folder baru untuk autentifikasi prometheus dan membuat password baru.

    ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/8.png)

10. Menambahkan auth_basic dan auth_basic_user_file di konfigurasi nginx untuk prometheus. 

    ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/9.png)

11. Cek hasilnya di prometheus.asep.onlinecamp.id dan masukkan username dan password yang sudah dikonfigurasikan sebelumnya.

    ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/10.png)
    ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Setup%20Monitoring%20Server/img/11.png)
