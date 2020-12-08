# Dumbways Bootcamp DevOps
## Week 1
### VM-Install Ubuntu

1. Untuk membuat Virtual Machine baru, klik "New".
    
    ![VM](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-1-BuatVMbaru.png)

2. Lalu beri nama untuk Virtual Machine baru, dan pilih versi Operating System.

    ![Nama](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-2-NamaVM.png)

3. Alokasikan ukuran RAM yang akan digunakan server. Disini digunakan 2 GB RAM.
    
    ![RAM](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-3-AlokasiRAM.png)

4. Buat Virtual Harddisk, dengan memilih "create a new virtual harddisk".

    ![VDI](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-4-MembuatVirtualHarddisk.png)

5. Pilih tipe Harddisk yang akan digunakan.
    
    ![tipeHDD](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-5-TipeHarddisk.png)

6. Alokasi tipe VDI pada physical HDD.

    ![tipeVDI](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-6-AlokasiPhysicalHDD.png)

7. Alokasikan ukuran Harddisk. Disini digunakan sebesar 10 GB.
    
    ![hddSize](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-7-AlokasiUkuranHDD.png)

8. Untuk memasukan ISO installer Ubuntu Server, klik setting.

    ![Setting](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-8-Setting.png)

9. Pilih ISO yang akan diinstall.
    
    ![ISO](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-9-PilihISO.png)

10. Start Virtual Machine.

    ![Start](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-10-StartVm.png)

11. Pilih bahasa yang digunakan.
    
    ![Bahasa](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-11-Bahasa.png)

12. Pilihan update Ubuntu. Karena tidak akan melakukan update, dipilih "Continue without updating".

    ![Update](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-12-pilihanUpdate.png)

13. Pilih Layout Keyboard.
    
    ![LayoutKB](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-13-KeyboardLayout.png)

14. Konfigurasi Proxy. Karena tidak menggunakan proxy manapun, dikosongkan saja

    ![Proxy](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-14-Proxy.png)

15. Konfigurasi Ubuntu Archive Mirror.
    
    ![Mirror](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-15-Mirror.png)

16. Konfigurasi storage. Karena akan dilakukan partisi secara manual, dipilih Custom lalu memilih HDD yang tersedia (VDI).

    ![Storage](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-16-AlokasiStorage.png)

17. Buat partisi pada server. Dialokasikan 1 GB untuk swap, dan 8,997 GB untuk root.
    
    ![partisi](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-17-Partisi.png)

18. Setup Profile.

    ![profile](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-18-SetupProfile.png)

19. Agar server dapat diremote, install OpenSSH.
    
    ![SSH](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-19-SSH.png)

20. Pilihan untuk menginstall aplikasi. Karena akan dilakukan secara manual satu per satu, step ini dilewati dengan tanpa memilih satupun.

    ![aplikasi](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-20-appserver.png)

21. Tunggu proses instalasi Server hingga selesai.

    ![Installing](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-21-Installing.png)

22. Setelah selesai, lakukan Login ke Server.

    ![Login](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-InstallUbuntu/img/1-22-login.png)