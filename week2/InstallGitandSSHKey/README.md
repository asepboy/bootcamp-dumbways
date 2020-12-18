# Dumbways Bootcamp DevOps
## Week 2
### Install Git and SSH Key

1. Fork project frontend dan backend
   
   ![1]()

   ![2]()

2. Buat 2 repository baru untuk project frontend dan backed
   
   ![3]()

   ![4]()

3. Buat instance baru yang jumlahnya disesuaikan dengan skema task (2 Frontend, 1 Backend, 1 Database). Dikarenakan melanjutkan dari task sebelumnya maka pada task ini perlu menambahkan 3 instance baru, yaitu Frontend, Backend, dan Database. Pada gambar dibawah ini diperlihatkan sebagian dari pembuatan instance. Semua instance baru ini dibuat private.
   
   ![5]()

   ![6]()

4. Pada setiap instance dilakukan command "ssh-keygen", untuk mengambil key SSH.
   
   ![7]()

5. copy isi file keygen, untuk didaftarkan pada Github.
   
   ![8]()

6. Pada github klik setting, lalu pilih menu "SSH and GPG Keys", lalu klik "New SSH Keys" untuk menambahkan SSH key dari setiap instance.
   
   ![9]()

7. Paste file keygen dari setiap instance
   
   ![10]()

8. Lalu akan muncul tampilan berikut, apabila sudah semua server dilakukan penambahan SSH key.
   
   ![11]()

9. Lalu lakukan "ssh -T git@github.com" pada semua server, untuk melakukan autentikasi.
    
    ![12]()

10. Lakukan clone project frontend dan backend, lalu masuk direktori project.
    
    ![13]()

11. Lakukan clone project. Push project tersebut ke repository yang tadi dibuat
    
    ![14]()

    ![15]()
