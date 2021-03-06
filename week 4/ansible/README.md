# Dumbways Bootcamp DevOps Batch 4
## Week 4
### Setup Server With Ansible

1. Membuat 6 Instance baru dan semuanya menggunakan docker kecuali nginx yang diantaranya: 
    - 1 server untuk nginx
    - 1 server untuk database
    - 4 server untuk proses instalasi (jenkins, monitoring,, frontend dan backend)
    
2. Melakukan proses instalasi ansible, disini saya menggunakan shell script untuk proses instalasinya.
    
    ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/1.png)

3. Mengubah file permission dengan command "chmod x+ ..." dan jalankan shell script "./ansible.sh"

    ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/2.png)
    
4. Membuat file inventory untuk dapat mengakses ke semua instance dengan ansible.

    ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/3.png)
    
5. Membuat file baru untuk default konfigurasi ansiblenya.

    ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/4.png)
    
6. Test koneksi ke semua instance dengan perintah "ansible all -m ping"

    ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/5.png)
    
7. Membuat file create_user.yml untuk membuat user baru untuk masing-masing instance.

    ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/6.png)
    
8. Jalankan create_user.yml dengan perintah "ansible-playbook create_user -bK".

    ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/7.png)
    
9. Melakukan proses Instalasi docker dan memberikan akses docker mengeksekusi tanpa root ke semua instance server dengan membuat file baru docker.yml

    ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/8.png)
    ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/9.png)
    
10. Jalankan file docker.yml dengan perintah "ansible-playbook docker.yml -bK"

    ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/10.png)
    
11. Membuat file baru untuk instalasi database dan jalankan dengan menggunakan perintah ansible-playbook.

     ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/11.png)
     
12. Membuat file baru untuk instalasi jenkins dan jalankan dengan menggunakan perintah ansible-playbook.
      
      ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/12.png)
      ![13](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/13.png)

13. Membuat file baru untuk instalasi prometheus, grafana dan node-exporter dan jalankan dengan menggunakan perintah ansible-playbook.

      ![14](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/14.png)
      ![15](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/15.png)

14. Membuat file baru untuk deployment frontend dan backend kemudian jalankan dengan perintah ansible-playbook.

      ![16](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/16.png)
      ![17](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%204/ansible/17.png)
