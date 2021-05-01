# Dumbways Bootcamp DevOps Batch 4
## Week 3
### Install Jenkins

1. - Membuat instance baru untuk jenkins.
   - Menginstal docker dan docker-compose di instance jenkins.
   - Membuat file baru docker-compese.yml
    
    ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/1.PNG)

2. Menjalankan docker-compose.yml di background.

    ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/2.PNG)
    ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/3.PNG)

3. Mendaftarkan sub domain di cloudflare.

    ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/4.PNG)
    
4. Membuat reverse proxy untuk jenkins.

    ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/5.PNG)
    ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/6.PNG)
  
5. Mendaftarkan SSL dengan certbot untuk sub domain yang sudah dibuat.

    ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/7.PNG)
    ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/8.PNG)
    
7. Mengambil password untuk jenkins di file directory instance jenkins docker.

    ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/9.PNG)
    ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/10.PNG)
    
8. Proses instalasi jenkins dan install plugin jenkins.

    ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/11.PNG)
    ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/12.PNG)
    
9. Membuat user baru untuk jenkins kemudian masukkan URL yang sudah didaftarkan subdomain cloudflare.

    ![13](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/13.PNG)
    ![14](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/14.PNG)
    ![15](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/15.PNG)
    ![16](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/16.PNG)
    
10. Menginstall publish over ssh di manage jenkins di dashboard kiri -> manage plugin -> publih over ssh -> download dan install plugin

    ![17](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/17.PNG)
    ![18](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/18.PNG)
    ![19](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/19.PNG)
    
11. Menambahkan Credentials global jenkins di manage jenkins di dashboard kiri -> manage credentials -> global credentials -> add credentials

    ![20](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/20.PNG)
    ![21](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/21.PNG)
    ![22](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/22.PNG)
    ![23](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/23.PNG)

12. Mengisi form dan memasukkan private key dari jenkins.

    ![24](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Install%20Jenkins/img/24.PNG)
    
    
