# Dumbways Bootcamp DevOps
## Final Task
### Webserver

1. Menginstall webserver nginx dan certbot untuk SSL.

  ```
  sudo apt install nginx
  sudo apt install software-properties-common
  sudo add-apt-repository ppa:certbot/certbot
  sudo apt install certbot python-certbot-nginx python3-certbot-dns-cloudflare
  ```

2. Membuat file konfigurasi nginx untuk frontend, backend, database, monitoring, prometheus dan jenkins. Kemudian edit file nginx.conf dan tambahkan include file directory dari masing-masing konfigurasi nginx.

   ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Webserver/1.png)
   
3. Mendaftarkan SSL dengan certbot dan URLnya untuk frontend, cicd, backend, monitoring dan prometheus.

   ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Webserver/2.png)

4. sebagai berikut hasil URL yang sudah dilakukan SSL dengan certbot :

   ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Webserver/3.png)
   ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Webserver/4.png)
   ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Webserver/5.png)
   ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Webserver/6.png)
   ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Webserver/7.png)
