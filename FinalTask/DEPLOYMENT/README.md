# Dumbways Bootcamp DevOps
## Final Task

### Deployment

1. Melakukan clone project backend dan frontend dari repo.
   
   ![1](/FinalTask/DEPLOYMENT/IMG/1.png)

2. Menjalankan playbook cloneRepo.yml
   
   ![2](/FinalTask/DEPLOYMENT/IMG/2.png)

3. Menjalankan docker-compose untuk frontend dan backend pada branch production.
   
   ![3](/FinalTask/DEPLOYMENT/IMG/3.png)

   ![4](/FinalTask/DEPLOYMENT/IMG/4.png)

4. Selanjutnya mengintegrasikan backend dengan database. Yang pertama dilakukan yaitu menyesuaikan credential pada production ke database. seperti pada gambar dibawah.
   
   ![5](/FinalTask/DEPLOYMENT/IMG/5.png)

5. Setelah itu install sequelize-cli. Sequelize adalah ORM yang digunakan node untuk mengintegrasikan dengan database.
   
   ![6](/FinalTask/DEPLOYMENT/IMG/6.png)

6. Lalu install depedency dari project tersebut.
   
   ![7](/FinalTask/DEPLOYMENT/IMG/7.png)

7. Setelah selesai, export NODE_ENV ke production, agar credential yang digunakan adalah production. Dan lakukan migrate database.
   
   ![9](/FinalTask/DEPLOYMENT/IMG/9.png)

8. Setelah selesai di backend, selanjutnya mengintegrasikan frontend dengan backend. Pada file /src/config/api.js ubah baseURL ke domain baru untuk API.
   
   ![10](/FinalTask/DEPLOYMENT/IMG/10.png)

9. Setelah itu akses domain yang telah dibuat untuk frontend, dan backend. Sebelumnya untuk pembuatan account menggunakan bantuan aplikasi postman.
    
    ![11](/FinalTask/DEPLOYMENT/IMG/11.png)

    ![12](/FinalTask/DEPLOYMENT/IMG/12.png)

    ![13](/FinalTask/DEPLOYMENT/IMG/13.png)