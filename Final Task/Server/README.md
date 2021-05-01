# Dumbways Bootcamp DevOps
## Final Task
### Server

1. Membuat VPC yang otomatis dapat dibuatkan untuk subnet public, subnet private, internet gateway serta NAT yang di elatic IP di "Wizard Launch VPC"
   
   ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/1.png)
   ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/2.png)

2. Berikut informasi yang sudah dibuatkan VPC, public subnet, private subnet, internet gateway dan NAT.

   ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/3.png)
   ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/4.png)
   ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/5.png)
   
3. Membuat Instance untuk Reverse Proxy, pilih ubuntu server.

   ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/6.png)
   
4. Memilih type instance yang "t2 micro"

   ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/7.png)

5. Pilih Network dengan VPC yang sudah dibuatkan, kemudiian subnetnya adalah public dan Auto-assign Public IP pilih Disable.

   ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/8.png)
   
6. Add storage untuk instancenya adalah 8GiB

   ![9](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/9.png)
   
7. Security Group dengan port 22, 443, dan 80.

   ![10](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/10.png)
   
8. Setelah instance untuk reverse proxy sudah dibuat, kemudian membuat instance untuk privatenya dengan Security Group adalah all traffic, sebagai berikut :
    - 2 instance untuk frontend 
    - 2 instance untuk backend 
    - 2 instance untuk database
    - 1 instance untuk jenkins/CICD
    - 1 instance untuk monitoring

   ![11](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/11.png)
   ![12](https://github.com/asepboy/bootcamp-dumbways/blob/main/Final%20Task/Server/12.png)
