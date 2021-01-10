# Dumbways Bootcamp DevOps
## Week 4
### Deploy PHP Application in cPanel

### Setup Grafana


1. Download CMS Vanilla Forums
2. Daftar infinityfree, lalu buat hosting account. pastikan dapat login vanillaforums.
   
   ![1]()

   ![2]()

   ![3]()

   ![4]()
    
3. Upload file vanilla forum ke infinityfree menggunakan filezilla. extract terlebih dahulu file yang sudah didownload.

    ![5]()

    ![6]()

4. Selanjutnya buat database, dan install vanilla forums melalui domain yang sudah didaftarkan.
   
   ![7]()

   ![8]()

   ![9]()

5. Selanjutnya daftarkan SSL untuk domain. Setup terlebih dahulu DNS record untuk domain, lalu setup CNAME. Sesuaikan source dan destination pada CNAME dengan DNS record.
   
   ![14]()

   ![15]()

6. Setelah itu tunggu beberapa saat untuk mendapatkan private key dan certificate. Hingga muncul seperti gambar dibawah.
   
   ![16]()

7. Setelah mendapatkan private key dan certificate copy pada SSL config di control panel, d=lalu upload.
   
   ![18]()

   ![17]()

8. Lalu pada client view tunggu hingga muncul status "Valid SSL Certificate is installed".

    ![19]()

9. Akses domain, dan pastikan cerficate sudah terinstall. (https://gilbran.freecluster.eu/)
    
    ![20]()