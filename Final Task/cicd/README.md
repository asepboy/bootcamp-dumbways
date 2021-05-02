# Dumbways Bootcamp DevOps
## Final Task
### CICD

1. Melakukan proses instalasi jenkins dengan menggunakan docker di ansible kemudian jalankan dengan menggunakan ansible-playbook.

   ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/1.png)

2. Mengambil InitialAdminPassword di dalam container docker jenkins dengan menggunakan command "docker exec -it jenkins bash" dan lakukan proses instalasi jenkins.

   ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/2.png)
   
3. Install plugin Publish over SSH.

   ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/3.png)
   
4. Menambahkan global credentials jenkins dan menambahkan private keys dari instance jenkins.

   ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/4.png)
   ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/5.png)
   
5. Menambahkan SSH Server di menu configure.

   ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/6.png)
   ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/7.png)
   ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/8.png)
   ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/9.png)
   
6. Menambahkan webhook github di masing-masing repository frontend dan backend.

   ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/10.png)
   
#### Create Jobs Frontend & Backend
7. Pilih create jobs -> freestyle project untuk proses cicd.
8. di tab "Source Code Management", isikan Repository URL dan credentials serta brance yang akan dibuild.

   ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/11.png)
   ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/12.png)
   
9. Ceklis pada Github hook trigger for GITScm polling.

   ![13](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/13.png)
   
10. Pada menu "Build" isikan dengan server name dan beberapa perintah yang akan dieksekusi oleh jenkins ketika ada code baru di push ke giithub.

   ![14](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/14.png)
   ![15](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/15.png)
   
11. Melakukan test CICD dengan mengubah file kemudian di push github.

   ![16](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/16.png)
   ![17](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/17.png)

12. Proses build otomatis dilakukan oleh jenkins ketika ada code baru yang di push ke github.

   ![18](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/18.png)
   
13. Hasil CICD yang sudah dibuild otomatis oleh jenkins.

   ![19](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/cicd/19.png)
