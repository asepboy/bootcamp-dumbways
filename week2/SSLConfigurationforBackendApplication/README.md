# Dumbways Bootcamp DevOps
## Week 2
### SSL Configuration for Backend Application

1. Karena sebelumnya certbot sudah diinstall, untuk selanjutnya hanya melakukan generate SSL untuk domain baru. Isi ketentuan berikutnya dari certbot.
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/1.png)

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/2.png)

2. Pada instance frontend, edit file api.js. Dengan merubah http menjadi https pada baseURL.
   
   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/3.png)

3. Setelah itu, coba akses domain via browser. pastikan ada logo gembok.
   
   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/7.png)
   
   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/12.png)

### Pengujian web Housy

1. Karena ketika proses signup pada housy gagal, disini menggunakan bantuan Postman untuk menguji API. Dengan method Get tambahkan link untuk signup.
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/4.png)

2. Setelah terkoneksi, ganti method dengan Post dan tambahkan script yang sesuai dengan field pada signup, seperti fullname, username, dsb.
   
   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/5.png)

3. Apabila berhasil, akan muncul seperti pada gambar berikut. Artinya user sudah berhasil ditambahkan.
   
   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/6.png)

4. Kembali ke web housy, lalu lakukan login dengan user yang baru ditambahkan,.
   
   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/7.png)

5. Selanjutnya coba add property, untuk menguji web housy. 
   
   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/8.png)

   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/9.png)

   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/10.png)

6. Lalu kembali ke Home, dan hasilnya sudah terlihat.
   
   ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SSLConfigurationforBackendApplication/img/11.png)