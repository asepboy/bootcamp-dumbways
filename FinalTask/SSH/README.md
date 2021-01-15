# Dumbways Bootcamp DevOps
## Final Task

### SSH

1. Membuat user yang sama untuk semua server. Disini saya menggunakan bantuan ansible, agar tidak mengulang. Untuk membuat password menggunakan bantuan aplikasi mkpasswd
   
   ![1](/FinalTask/SSH/IMG/1.png)

2. Eksekusi file ansible playbook.
   
   ![2](/FinalTask/SSH/IMG/2.png)

3. Buat user agi di server ansible.
   
   ![3](/FinalTask/SSH/IMG/3.png)

4. Setelah itu generate SSH-Key
   
   ![4](/FinalTask/SSH/IMG/4.png)

5. Lalu ubah nama SSH key menjadi ```<inisial>@dumbways```

6. Login ke Server monitoring dengan user yang sama, lalu lakukan ```ssh-keygen``` lalu exit.
   
   ![7](/FinalTask/SSH/IMG/7.png)

   ![8](/FinalTask/SSH/IMG/8.png)

7. Setelah itu copy SSH-key dari ansible ke server monitoring. Setelah selesai login hanya dengan menggunakan IP
   
   ![9](/FinalTask/SSH/IMG/9.png)