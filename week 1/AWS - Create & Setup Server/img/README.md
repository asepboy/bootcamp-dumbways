# Dumbways Bootcamp DevOps Batch 4
## Week 1 - day 1
### VM-Install Application

1. Disini saya akan membuat 2 yaitu instance untuk reverse proxy dan instance untuk aplikasi. pertama saya buat instance untuk reverse proxy, Klik Launch a virtual machine EC2 pada menu dashboard aws. 
    
    ![update](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/1.PNG)

2. Amazon Machine Image cari dan pilih ubuntu server, disini saya pilih ubuntu server 18.04 LTS.
    
    ![curl](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/2.PNG)

3. Pilih instance type.
    
    ![install](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/3.PNG)

4. Konfigurasi instance dengan pilih network, subnet dan disini saya "disable" untuk Auto-assign Public IP.
    
    ![clone](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/4.PNG)

5. Tentukan ukuran storage yang akan digunakan pada instance.
    
    ![ls](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/5.PNG)

6. Konfigurasikan Security Group untuk kebutuhan proxy dengan membuka port 22, 80 dan 443.
    
    ![npmInstall](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/6.PNG)

7. Review Instance dan klik launch.
    
    ![npmStart](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/7.PNG)

8. pilih Create a new key pair dan isi nama key pair kemudian download, simpan keypair ditempat yang aman.

    ![browser](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/8.PNG)

9. Ubah nama instance supaya memudahkan dalam menatanya.

    ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/9.PNG)

10. Untuk mendapatkan IP Public pada instance, klik Allocate Elastic IP address.

    ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/10.PNG)

11. Klik Allocate untuk merequest IP.

    ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/11.PNG)

12. Associate Elastic IP Adderess pada public instance, dan Public IP sudah didapatkan untuk instance reverse proxy. 

    ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/12.PNG)
    ![13](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/13.PNG)

13. Selanjutnya lakukan hal yang sama untuk membuat instance aplikasi, dengan port All Trafic dan port 3000 untuk aplikasinya.

    ![14](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/14.PNG)
    
14. Selanjutnya melakukan remote ke Public instance, ubah akses keypair yg sudah didownload dengan chmod 400.

    ![15](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/15.PNG)
    
15. Gunakan SSH untuk meremote public instance dengan keypair tersebut.

    ![16](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/16.PNG)
    ![17](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/17.PNG)
 
16. Tambahkan user pada public instance.

    ![18](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/18.PNG)    

17. Masukan user baru ke grup sudo, dan berikan akses super user.

    ![19](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/19.PNG)

18. Edit file konfigurasi ssh agar dapat melakukan remote instance tanpa menggunakan keypair. Pada PasswordAuthentication ubah jadi yes. 

    ![20](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/20.PNG)
    ![21](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/21.PNG)

19. Kemudian lakukan restart ssh.
    
    ![22](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/22.PNG)
    
20. Keluar dari public instance, dan lakukan test remote instance tanpa menggunakan keypair.

    ![23](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/23.PNG)
    ![24](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/24.PNG)

   ### VM-Install Application
   
21. mengirimkan keypair dari local komputer ke public instance dengan menggunakan perintah scp.
 
    ![25](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/25.PNG)

22. Test remote SSH instance untuk aplikasi yang sudah dibuat melalui instance proxy public instance.

    ![26](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Create%20%26%20Setup%20Server/img/26.PNG)
    
    
