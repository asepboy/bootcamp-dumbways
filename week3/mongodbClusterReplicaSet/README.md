# Dumbways Bootcamp DevOps
## Week 3 (Additional Task)
### Clustering Database with MongoDB Replica Set

1. Install MongoDB
    - Import Public Key
        
        ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/1.png)

    - Create a list for MongoDB

        ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/2.png)

    - Update package 
        
        ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/3.png)

    - Install MongoDB

        ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/4.png)

    - Start MongoDB

        ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/5.png)

2. Konfigurasi Replica Set
    - Clone VM menjadi 3 VM (1 Primary dan 2 Secondary)

        ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/11.png)

        ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/12.png)


    - Tambahkan Hostname di /etc/hosts. Masukan seluruh IP dari Host

        ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/13.png)

        ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/14.png)

        ![15](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/15.png)

    - Tambahkan bindIP dan replSetname pada setiap Host di /etc/mongo/mongod.conf.

        ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/6.png)

        ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/7.png)

        ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/8.png)

    - Ping antar Host, untuk memastikan host sudah saling terhubung.

        ![16](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/16.png)

        ![17](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/17.png)

        ![18](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/18.png)

    - Initiate Replication Set
      - Primary
        - Login mongoDB

            ![22](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/22.png)

        - initiate 

            ![23](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/23.png)

        - add secondary

            ![24](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/24.png)

            ![25](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/25.png)

      - Secondary
        - Konfirmasi secondary

            ![37](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/37.png)

      - Primary
        - cek status

            ![26](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/26.png)
            
            ![27](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/27.png)
            
            ![28](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/28.png)

            ![29](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/29.png)

3. Testing Replication Set
    - Primary
      - Buat Database, dan isi database baru tersebut
            
        ![30](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/30.png)


  
    - Secondary
      - cek isi database
                
        ![31](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/31.png)

        ![32](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/mongodbClusterReplicaSet/img/32.png)