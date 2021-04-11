# Dumbways Bootcamp DevOps
## Week 1
### AWS-SSL Configuration

1. Cek package update terakhir
   
   ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20SSL%20Configuration/img/1.PNG)

2. tambah repo ppa certbot
   
   ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20SSL%20Configuration/img/2.PNG)

3. Install certbot
   
   ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20SSL%20Configuration/img/3.PNG)

4. Daftarkan domain ke certbot. Lalu isikan email, agreement, dsb.
   
   ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20SSL%20Configuration/img/4.PNG)
   ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20SSL%20Configuration/img/5.PNG)

5. Setelah selesai, cek pada konfigurasi reverse proxy (/etc/nginx/asep/..). Pastikan SSL telah diterapkan.

    ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20SSL%20Configuration/img/6.PNG)

6. Akses project menggunakan domain pada browser.

    ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20SSL%20Configuration/img/7.PNG)
