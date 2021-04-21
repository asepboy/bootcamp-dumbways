# Dumbways Bootcamp DevOps Batch 4
## Week 3
### Create Jenkins Job

1. Konfigurasi publish over ssh di manage jenkins -> configure system -> publish over ssh -> add servers.
    
    ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/1.PNG)
    ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/2.PNG)
    
2. Isi ssh server pada masing-masing frontend dan backend.

    ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/3.PNG)
    ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/4.PNG)
    
3. Membuat freestyle project untuk frontend dan backend.

    ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/3.PNG)

4. Pada tab source code management di isi url project github.

    ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/6.png)

5. Ceklis pada tab build trigger untuk melakukan hook trigger ke github.

    ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/7.PNG)

6. Pada tab build mengisi beberapa perintah yang akan dilakukan oleh jenkins.

    ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/8.png)
    
7. Klik advance dan ubah exec timeout menjadi 0

    ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/9.png)
    
8. untuk backend sama konfigurasinya, yang berbeda hanya URL git dan exec command pada freestyle project.

    ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/10.png)
    
9. freestyle project untuk frontend dan backend sudah dibuat.

    ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/11.png)
    
10. Melakukan webhook di docker hub untuk repo frontend dan backend.

    ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/12.png)
    ![13](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/13.png)
    
11. membuat webhook di github untuk repo frontend dan backend.

    ![14](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/14.PNG)
    ![15](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/15.png)
    
12. Menguji project jenkins dengan build now.

    ![16](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/16.png)
    ![17](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/17.png)
    
13. Mengintegrasi jenkins dan notifikasi slack. Menginstall plugin Notifikasi Slack di jenkins dan menginstall jenkins di slack.

    ![18](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/18.png)
    ![19](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/19.png)
    
14. Pada manage credential jenkins tambah credential untuk slack.

    ![20](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/20.png)
    
15. Proses integrasi masuk ke manage jenkins -> configure system. Masukkan form dan credential untuk slack

    ![21](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/21.png)
    
16. Uji project dengan build now.

    ![22](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/22.png)
    
17. Notifikasi berhasil di slack.

    ![23](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%203/Create%20Jenkins%20Job/img/23.png)
