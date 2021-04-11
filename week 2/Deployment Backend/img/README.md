# Dumbways Bootcamp DevOps
## Week 2
### Deployment Backend

1. clone repository backend dengan perintah `https://github.com/asepboy/wayshub-backend.git` kemudian masuk ke directory `cd wayshub-backend/` dan masuk via SSH dengan perintah `git remote add origin git@github.com:asepboy/wayshub-backend1.git`

2. Instal library seperti pada bagian frontend seperti nodejs, npm, pm2, dan tambahan sequelize untuk kebutuhan migrasi database
- `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash`
- `npm install 14`
- `npm install pm2 -g`
- `npm install -g sequelize-cli`

3. Masuk ke directory `~/wayshub-backend/config` untuk edit file `config.json` sesuai username, password, database, dan IP private server database

    ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Deployment%20Backend/img/1.PNG)

4. Buat database baru untuk wayshub. 

    ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Deployment%20Backend/img/2.PNG)

5. Migrasi database dengan perintah `sequelize db:migrate`

    ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Deployment%20Backend/img/3.PNG)

6. Kemudian jalankan pm2
- `pm2 --name Wayhub-backend start npm -- start`
