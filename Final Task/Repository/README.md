# Dumbways Bootcamp DevOps Batch 4
## Final Task
### Repository

1. Mempersiapkan repository frontend dan backend, diantaranya :
    - Melakukan clone repo frontend dan backend :
        ```
        git clone https://github.com/sgnd/waysgallery-frontend  
        git clone https://github.com/sgnd/waysgallery-backend
        ```
     
     ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Repository/2.png)
     
2. Membuat branch production dan development di frontend dan backend.
    - git branch development
    - git branch production 
    
    ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Repository/3.png)

3. Push repository public yang sudah dibuat ke repository private milik pribadi dan menghapus yang public di server.
    - git push --mirror git@github.com:asepboy/waysgallery-frontend.git
    - git push --mirror git@github.com:asepboy/waysgallery-backend.git
    - cd .. 
    - rm -rf waysgallery-frontend 
    - rm -rf waysgallery-backend

4. Menambahkan SSH masing-masing instance frontend dan backend ke SSH github.

    ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Repository/4.png)
    ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Repository/5.png)
    
5. Melakukan clone repository ulang ke repository private, dan lakukan test remote, pull dan push.
    - git clone git@github.com:asepboy/waysgallery-frontend.git
    - git clone git@github.com:asepboy/waysgallery-backend.git

    ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Repository/6.png)
