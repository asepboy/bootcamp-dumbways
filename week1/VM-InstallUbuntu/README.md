# Dumbways Bootcamp DevOps
## Week 1
### VM-Install Ubuntu

1. Untuk membuat Virtual Machine baru, klik "New".
    
    ![VM]()

2. Lalu beri nama untuk Virtual Machine baru, dan pilih versi Operating System.

    ![Nama]()

3. Alokasikan ukuran RAM yang akan digunakan server. Disini digunakan 2 GB RAM.
    
    ![RAM]()

4. Buat Virtual Harddisk, dengan memilih "create a new virtual harddisk".

    ![VDI]()

5. Pilih tipe Harddisk yang akan digunakan.
    
    ![tipeHDD]()

6. Alokasi tipe VDI pada physical HDD.

    ![tipeVDI]()

7. Alokasikan ukuran Harddisk. Disini digunakan sebesar 10 GB.
    
    ![hddSize]()

8. Untuk memasukan ISO installer Ubuntu Server, klik setting.

    ![Setting]()

9. Pilih ISO yang akan diinstall.
    
    ![ISO]()

10. Start Virtual Machine.

    ![Start]()

11. Pilih bahasa yang digunakan.
    
    ![Bahasa]()

12. Pilihan update Ubuntu. Karena tidak akan melakukan update, dipilih "Continue without updating".

    ![Update]()

13. Pilih Layout Keyboard.
    
    ![LayoutKB]()

14. Konfigurasi Proxy. Karena tidak menggunakan proxy manapun, dikosongkan saja

    ![Proxy]()

15. Konfigurasi Ubuntu Archive Mirror.
    
    ![Mirror]()

16. Konfigurasi storage. Karena akan dilakukan partisi secara manual, dipilih Custom lalu memilih HDD yang tersedia (VDI).

    ![Storage]()

17. Buat partisi pada server. Dialokasikan 1 GB untuk swap, dan 8,997 GB untuk root.
    
    ![partisi]()

18. Setup Profile.

    ![profile]()

19. Agar server dapat diremote, install OpenSSH.
    
    ![SSH]()

20. Pilihan untuk menginstall aplikasi. Karena akan dilakukan secara manual satu per satu, step ini dilewati dengan tanpa memilih satupun.

    ![aplikasi]()

21. Tunggu proses instalasi Server hingga selesai.

    ![Installing]()

22. Setelah selesai, lakukan Login ke Server.

    ![Login]()