# Dumbways Bootcamp DevOps
## Final Task

### Database

1. Database yang digunakan adalah MariaDB cluster, dengan 2 buah container master dan slave. Yang pertama dilakukan adalah menginstall docker. Pada instalasi ini menggunakan bantuan ansible, sehingga semua server yang menggunakan layanan docker terinstall secara bersamaan. Pada gambar dibawah diperlihatkan konfigurasi untuk menginstall docker dan memasukan user yang terdaftar pada Inventory file dan juga menginstall docker-compose. 
   
   ![1](/FinalTask/DATABASE/IMG/1.png)

2. Lalu eksekusi file playbook docker.
   
   ![2](/FinalTask/DATABASE/IMG/2.png)

3. Setelah itu lakukan clone repo database, sebelumnya saya sudah membuat file docker compose untuk database ini dan disimpan digithub.
   
   ![3](/FinalTask/DATABASE/IMG/3.png)

4. Lalu eksekusi file playbook untuk clone repo.
   
   ![4](/FinalTask/DATABASE/IMG/4.png)

5. Karena database menggunakan docker maka selanjutnya menjalankan docker untuk layanan database. menjalankan docker juga menggunakan ansible sehingga dapat dilakukan secara bersamaan. Gambar berikut memperlihatkan playbook untuk menjalankan docker.
   
   ![5](/FinalTask/DATABASE/IMG/5.png)

6. Selanjutnya menjalankan ansible playbook untuk runDocker.yml
   
   ![6](/FinalTask/DATABASE/IMG/6.png)

7. Gambar dibawah memperlihatkan database sudah berjalan, dengan 2 buah container, yaitu master dan slave.
   
   ![7](/FinalTask/DATABASE/IMG/7.png)

8. Selanjutnya menambahkan load balancing untuk database menggunakan HAProxy. Install terlebih dahulu HA Proxy lalu tambahkan rules berikut di /etc/haproxy/haproxy.conf
   
   ![8](/FinalTask/DATABASE/IMG/8.png)

9. Setelah itu untuk memastikan database dapat digunakan, dilakukan remote dari server backend.
    
    ![9](/FinalTask/DATABASE/IMG/9.png)

10. Selanjutnya melakukan migrate dari backend, dengan perintah sequelize db:migrate
    
    ![10](/FinalTask/DATABASE/IMG/10.png)