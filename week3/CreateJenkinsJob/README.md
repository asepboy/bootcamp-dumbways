# Dumbways Bootcamp DevOps
## Week 3
### Create Jenkins Job

1. Unlock Jenkins, dengan command seperti dibawah.
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/1.png)

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/2.png)

   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/3.png)

2. Install Plugins pada Jenkins.
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/4.png)

   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/5.png)

3. Set user untuk Admin, dan masukan Jenkins URL. Dan Jenkins siap digunakan.
   
   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/6.png)

   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/7.png)
   
   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/8.png)

4. Instal Plugin "Publis over SSH" agar Jenkins dapat melakukan remote ke Server tujuan. Setelah didownload tunggu Jenkins melakukan restart.
   
   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/9.png)

   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/10.png)

   ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/11.png)

   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/12.png)

5. Buat Credential untuk Server Jenkins. Pada field username dan Private Key, masukan username yang ada pada server jenkins, dan masukan private key dari jenkins server.
   
   ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/13.png)
   
   ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/14.png)

   ![15](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/15.png)

   ![16](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/16.png)

   ![17](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/17.png)

6. Selanjutnya memasukan data server yang akan diremote oleh Jenkins. Masukan seluruh server (2 Frontend dan 1 Backend).
   
   ![19](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/19.png)

   ![20](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/20.png)

    #### Backend
    ![21](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/Backend/21.png)

    #### Frontend1
    ![21](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/21.png)

    #### Frontend2
    ![21](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/Frontend2/21.png)

7. Membuat Job Jenkins. Job yang dibuat ada 3 yaitu untuk Backend, Frontend1, dan Frontend2. Pada tipe job dipilih freestyle projet. Lalu memasukan url git dari repo yang digunakan, karena Github digunakan sebagai trigger. Pada step Build dipilih "Send files or command over SSH" sehingga jenkins dapat melakukan remote ke server yang bersangkutan. Lalu memberikan command yang disesuaikan dengan kebutuhan.
   
   ![22](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/22.png)

   ![23](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/23.png)

    #### Frontend1
   ![24](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/24.png)

   ![25](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/25.png)

   ![26](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/26.png)

   ![27](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/27.png)

   ![28](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/28.png)

   #### Frontend2

   ![24](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/Frontend2/24.png)
   
   ![27](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/Frontend2/27.png)    

   #### Backend

   ![24](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/Backend/24.png)
   
   ![27](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/Backend/27.png)  

8. Selanjutnya membuat webhooks untuk Jenkins. Agar trigger dapat dilakukan dari Github.
   
   ![28](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/28.png)
   
   ![29](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/29.png)

   ![30](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/30.png)
   
   ![31](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/31.png)    

   #### Backend

   ![30](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/Backend/30.png)
   
9. Lalu melakukan pengujian trigger dari Github.

   ![34](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/34.png)
   
   ![35](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/35.png)

   ![36](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/36.png) 

10. Menghubungkan Github ke Docker Hub. Pada dashboard docker terlihat aktifitas yang telah dilakukan.
    
    ![41](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/41.png)

    ![42](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/42.png)

    ![38](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/38.png)

    ![39](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/CreateJenkinsJob/img/39.png)
   

### Email Notification

1. Pastikan email dapat diakses melalui Jenkins. Allow Less Secure App di on kan.
   
   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/2.png)

   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/3.png)

2. Isi field pada Extended Email Configuration sesuai dengan ketentuan. 
   
   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/9.png)

   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/10.png)

3. Lalu pada setiap job tambahkan Post-build Action dengan action Editable Email Notification. Trigger yang digunakan adalah Always, sehingga apapun status yang dihasilkan akan langsung dikirim ke email yang telah didaftarkan.
   
   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/12.png)

   ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/13.png)

4. Percobaan Notifikasi Email. Terdapat 2 percobaan yaitu Notifikasi Success dan gagal atau unstable.
   
   ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/14.png)
   
   ![15](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/15.png)

   ![16](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/16.png)

   ![17](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/17.png)

   ![18](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/18.png)

   ![19](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/19.png)

   ![20](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/emailNotif/img/20.png)
   