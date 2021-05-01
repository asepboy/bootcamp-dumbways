# Dumbways Bootcamp DevOps Batch 4
## Week 4
### Deploy PHP Applications in Cpanel

1. Platform yang digunakan antara lain :
    - CMS : Vanilla Forum CMS
    - Cpanel : InfinityFree Cpanel
    - FTP : Filezilla
    - Domain : asep.infinityfreeapp.com
    - SSL : Lets Encrypt dari Infinityfree


2. Daftar hosting di Infinityfree Hosting, kemudian create hosting dan subdomainnya.
    
    ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/1.png)
    
3. Membuat password untuk hostingnya.
    
    ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/2.png)

4. Hosting sudah dibuat dan pilih Open Control Panel.

    ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/3.png)
    ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/4.png)
    
5. 	Buka Filezilla yang sudah terinstall dan masukkan Host, username, password dan portnya.

    ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/5.png)
    
6. Download Vanilla Forum CMS kemudian extract file. Buka folder package yang sudah di extract file dari vanilla forum cms kemudian pilih semua file dan drag and drop dari package ke folder htdocs yang ada di hosting.

    ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/6.png)
    
7.  Menambahkan database di hosting cpanelnya.

    ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/7.png)
    
8. Ketika proses upload dengan filezilla sudah selesai, maka buka subdomain di browser kemudian lakukan proses konfigurasi database yang sudah dibuat dan lakukan proses instalasi cmsnya.

    ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/8.png)
    
9. Menambahkan SSL untuk subdomainnya. 

    ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/9.png)
    
10. SSL untuk subdomain sudah direquest.

    ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/10.png)
    
11. Menambahkan Custom CNAME Record DNS di CNAME Cpanel dan masukkan Record Name, Domain dan Destination dari DNS Record Infinityfree.

    ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/11.png)
    
12. Setelah itu tunggu beberapa saat untuk mendapatkan private keys dan certificate keys dari infinity free.

    ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/12.png)
    
13. Menambahkan private keys dan certificate keys dari infinityfree ke SSL/TLS Cpanel.

    ![13](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/13.png)
    
14. Hasil subdomain yang sudah di SSL.

    ![14](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/Deploy%20PHP%20Applications%20in%20Cpanel/img/14.png)
    
