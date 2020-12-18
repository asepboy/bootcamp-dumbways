# Dumbways Bootcamp DevOps
## Week 2
### Install Git and SSH Key

1. Fork project frontend dan backend
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/1.png)

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/2.png)

2. Buat 2 repository baru untuk project frontend dan backed
   
   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/3.png)

   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/4.png)

3. Buat instance baru yang jumlahnya disesuaikan dengan skema task (2 Frontend, 1 Backend, 1 Database). Dikarenakan melanjutkan dari task sebelumnya maka pada task ini perlu menambahkan 3 instance baru, yaitu Frontend, Backend, dan Database. Pada gambar dibawah ini diperlihatkan sebagian dari pembuatan instance. Semua instance baru ini dibuat private.
   
   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/5.png)

   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/6.png)

4. Pada setiap instance dilakukan command "ssh-keygen", untuk mengambil key SSH.
   
   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/7.png)

5. copy isi file keygen, untuk didaftarkan pada Github.
   
   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/8.png)

6. Pada github klik setting, lalu pilih menu "SSH and GPG Keys", lalu klik "New SSH Keys" untuk menambahkan SSH key dari setiap instance.
   
   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/9.png)

7. Paste file keygen dari setiap instance
   
   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/10.png)

8. Lalu akan muncul tampilan berikut, apabila sudah semua server dilakukan penambahan SSH key.
   
   ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/11.png)

9. Lalu lakukan "ssh -T git@github.com" pada semua server, untuk melakukan autentikasi.
    
    ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/12.png)

10. Lakukan clone project frontend dan backend, lalu masuk direktori project.
    
    ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/13.png)

11. Lakukan clone project. Push project tersebut ke repository yang tadi dibuat
    
    ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/14.png)

    ![15](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/InstallGitandSSHKey/img/15.png)
