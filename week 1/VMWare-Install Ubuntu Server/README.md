# Dumbways Bootcamp DevOps Batch 4
## Week 1 - day 1
### VM-Install Ubuntu

1. Untuk membuat Virtual Machine baru, klik "New".
    
    ![VM](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/1.PNG)

2. Lalu beri nama untuk Virtual Machine baru, dan pilih versi Operating System.

    ![Nama](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/2.PNG)

3. Alokasikan ukuran RAM yang akan digunakan server. Disini digunakan 2 GB RAM.
    
    ![RAM](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/3.PNG)

4. Buat Virtual Harddisk, dengan memilih "Create a virtual harddisk now".

    ![VDI](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/4.PNG)

5. Pilih tipe Harddisk yang akan digunakan.
    
    ![tipeHDD](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/5.PNG)

6. Alokasi tipe VDI pada physical HDD.

    ![tipeVDI](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/6.PNG)

7. Alokasikan ukuran Harddisk. Disini digunakan sebesar 10 GB.
    
    ![hddSize](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/7.PNG)

8. Untuk memasukan ISO installer Ubuntu Server, klik setting.

    ![Setting](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/8.PNG)

9. Pilih ISO yang akan diinstall.
    
    ![ISO](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/9.png)

10. Start Virtual Machine.

    ![Start](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/10.PNG)

11. Pilih bahasa yang digunakan.
    
    ![Bahasa](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/11.PNG)

12. Pilihan update Ubuntu. Karena tidak akan melakukan update, dipilih "Continue without updating".

    ![Update](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/12.PNG)

13. Pilih Layout Keyboard.
    
    ![LayoutKB](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/13.PNG)

14. Konfigurasi Proxy. Karena tidak menggunakan proxy manapun, dikosongkan saja

    ![Proxy](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/14.PNG)

15. Konfigurasi Ubuntu Archive Mirror.
    
    ![Mirror](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/15.PNG)

16. Konfigurasi storage. Karena akan dilakukan partisi secara manual, dipilih Custom lalu memilih HDD yang tersedia (VDI).

    ![Storage](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/16.PNG)

17. Buat partisi pada server. Dialokasikan 1 GB untuk swap, dan 8,997 GB untuk root.
    
    ![partisi](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/17.PNG)

18. Setup Profile.

    ![profile](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/18.PNG)

19. Agar server dapat diremote, install OpenSSH.
    
    ![SSH](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/19.PNG)

20. Pilihan untuk menginstall aplikasi. Karena akan dilakukan secara manual satu per satu, step ini dilewati dengan tanpa memilih satupun.

    ![aplikasi](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/20.PNG)

21. Tunggu proses instalasi Server hingga selesai.

    ![Installing](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/21.PNG)

22. Setelah selesai, lakukan Login ke Server.

    ![Login](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Install%20Ubuntu%20Server/img/22.PNG)
