# Dumbways Bootcamp DevOps
## Week 2
### Install Git and SSH Key

1. Fork project frontend dan backend
   
   ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/2.PNG)

2. Buat repository baru 
   
   ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/2.PNG)

3. Clone repository backend public yang sudah di fork ke server backend dan buat repository private baru di akun github untuk push isi dari repository public ke repository private dengan git clone --bare, kemudian cd library-backend.git dan git push --mirror 
   
   ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/3.PNG)

4. Clone repository private ke server backend dengan git clone.
   
   ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/4.PNG)

5. Instal key untuk login git via SSH sehingga tidak perlu menggunakan username dan password. ssh-keygen -C kemudian cd .ssh/ Cat id_rsa.pub.
   
   ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/5.PNG)

6. Copy isi dari file id_rsa.pub ke git.
   
   ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/6.PNG)

7. Pastikan SSH key sudah terpasang di server.
   
   ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/7.PNG)

8. Hapus git yang di remote kemudian login ulang menggunakan SSH key.
   
   ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/8.PNG)

9. Tes fungsi git pull, git commit, dan git push tanpa menggunakan password
    
    ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/9.PNG)
    ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/10.PNG)
    ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/11.PNG)
    ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Install%20Git%20dan%20SSH/img/12.PNG)
