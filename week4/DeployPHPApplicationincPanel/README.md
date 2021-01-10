# Dumbways Bootcamp DevOps
## Week 4
### Deploy PHP Application in cPanel



1. Download CMS Vanilla Forums
2. Daftar infinityfree, lalu buat hosting account. pastikan dapat login vanillaforums.
   
   ![1](/week4/DeployPHPApplicationincPanel/img/1.png)

   ![2](/week4/DeployPHPApplicationincPanel/img/2.png)

   ![3](/week4/DeployPHPApplicationincPanel/img/3.png)

   ![4](/week4/DeployPHPApplicationincPanel/img/4.png)
    
3. Upload file vanilla forum ke infinityfree menggunakan filezilla. extract terlebih dahulu file yang sudah didownload.

    ![5](/week4/DeployPHPApplicationincPanel/img/5.png)

    ![6](/week4/DeployPHPApplicationincPanel/img/6.png)

4. Selanjutnya buat database, dan install vanilla forums melalui domain yang sudah didaftarkan.
   
   ![7](/week4/DeployPHPApplicationincPanel/img/7.png)

   ![8](/week4/DeployPHPApplicationincPanel/img/8.png)

   ![9](/week4/DeployPHPApplicationincPanel/img/9.png)

5. Selanjutnya daftarkan SSL untuk domain. Setup terlebih dahulu DNS record untuk domain, lalu setup CNAME. Sesuaikan source dan destination pada CNAME dengan DNS record.
   
   ![14](/week4/DeployPHPApplicationincPanel/img/14.png)

   ![15](/week4/DeployPHPApplicationincPanel/img/15.png)

6. Setelah itu tunggu beberapa saat untuk mendapatkan private key dan certificate. Hingga muncul seperti gambar dibawah.
   
   ![16](/week4/DeployPHPApplicationincPanel/img/16.png)

7. Setelah mendapatkan private key dan certificate copy pada SSL config di control panel, d=lalu upload.
   
   ![18](/week4/DeployPHPApplicationincPanel/img/18.png)

   ![17](/week4/DeployPHPApplicationincPanel/img/17.png)

8. Lalu pada client view tunggu hingga muncul status "Valid SSL Certificate is installed".

    ![19](/week4/DeployPHPApplicationincPanel/img/19.png)

9. Akses domain, dan pastikan cerficate sudah terinstall. (https://gilbran.freecluster.eu/)
    
    ![20](/week4/DeployPHPApplicationincPanel/img/20.png)