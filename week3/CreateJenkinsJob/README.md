# Dumbways Bootcamp DevOps
## Week 3
### Create Jenkins Job

1. Unlock Jenkins, dengan command seperti dibawah.
   
   ![1]()

   ![2]()

   ![3]()

2. Install Plugins pada Jenkins.
   
   ![4]()

   ![5]()

3. Set user untuk Admin, dan masukan Jenkins URL. Dan Jenkins siap digunakan.
   
   ![6]()

   ![7]()
   
   ![8]()

4. Instal Plugin "Publis over SSH" agar Jenkins dapat melakukan remote ke Server tujuan. Setelah didownload tunggu Jenkins melakukan restart.
   
   ![9]()

   ![10]()

   ![11]()

   ![12]()

5. Buat Credential untuk Server Jenkins. Pada field username dan Private Key, masukan username yang ada pada server jenkins, dan masukan private key dari jenkins server.
   
   ![13]()
   
   ![14]()

   ![15]()

   ![16]()

   ![17]()

6. Selanjutnya memasukan data server yang akan diremote oleh Jenkins. Masukan seluruh server (2 Frontend dan 1 Backend).
   
   ![19]()

   ![20]()

    #### Backend
    ![21]()

    #### Frontend1
    ![21]()

    #### Frontend2
    ![21]()

7. Membuat Job Jenkins. Job yang dibuat ada 3 yaitu untuk Backend, Frontend1, dan Frontend2. Pada tipe job dipilih freestyle projet. Lalu memasukan url git dari repo yang digunakan, karena Github digunakan sebagai trigger. Pada step Build dipilih "Send files or command over SSH" sehingga jenkins dapat melakukan remote ke server yang bersangkutan. Lalu memberikan command yang disesuaikan dengan kebutuhan.
   
   ![22]()

   ![23]()

    #### Frontend1
   ![24]()

   ![25]()

   ![26]()

   ![27]()

   ![28]()

   #### Frontend2

   ![24]()
   
   ![27]()    

   #### Backend

   ![24]()
   
   ![27]()  

8. Selanjutnya membuat webhooks untuk Jenkins. Agar trigger dapat dilakukan dari Github.
   
   ![28]()
   
   ![29]()

   ![30]()
   
   ![31]()    

   #### Backend

   ![30]()
   
9. Lalu melakukan pengujian trigger dari Github.

   ![34]()
   
   ![35]()

   ![36]() 

10. Menghubungkan Github ke Docker Hub. Pada dashboard docker terlihat aktifitas yang telah dilakukan.
    
    ![41]()

    ![42]()

    ![38]()

    ![39]()
   

### Email Notification

1. Pastikan email dapat diakses melalui Jenkins. Allow Less Secure App di on kan.
   
   ![2]()

   ![3]()

2. Isi field pada Extended Email Configuration sesuai dengan ketentuan. 
   
   ![9]()

   ![10]()

3. Lalu pada setiap job tambahkan Post-build Action dengan action Editable Email Notification. Trigger yang digunakan adalah Always, sehingga apapun status yang dihasilkan akan langsung dikirim ke email yang telah didaftarkan.
   
   ![12]()

   ![13]()

4. Percobaan Notifikasi Email. Terdapat 2 percobaan yaitu Notifikasi Success dan gagal atau unstable.
   
   ![14]()

   ![15]()

   ![16]()

   ![17]()

   ![18]()

   ![19]()

   ![20]()
   