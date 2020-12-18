# Dumbways Bootcamp DevOps
## Week 2
### SSL Configuration for Backend Application

1. Karena sebelumnya certbot sudah diinstall, untuk selanjutnya hanya melakukan generate SSL untuk domain baru. Isi ketentuan berikutnya dari certbot.
   
   ![1]()

   ![2]()

2. Pada instance frontend, edit file api.js. Dengan merubah http menjadi https pada baseURL.
   
   ![3]()

3. Setelah itu, coba akses domain via browser. pastikan ada logo gembok.
   
   ![7]()
   
   ![12]()

### Pengujian web Housy

1. Karena ketika proses signup pada housy gagal, disini menggunakan bantuan Postman untuk menguji API. Dengan method Get tambahkan link untuk signup.
   
   ![4]()

2. Setelah terkoneksi, ganti method dengan Post dan tambahkan script yang sesuai dengan field pada signup, seperti fullname, username, dsb.
   
   ![5]()

3. Apabila berhasil, akan muncul seperti pada gambar berikut. Artinya user sudah berhasil ditambahkan.
   
   ![6]()

4. Kembali ke web housy, lalu lakukan login dengan user yang baru ditambahkan,.
   
   ![7]()

5. Selanjutnya coba add property, untuk menguji web housy. 
   
   ![8]()

   ![9]()

   ![10]()

6. Lalu kembali ke Home, dan hasilnya sudah terlihat.
   
   ![11]()