# Dumbways Bootcamp DevOps Batch 4
## Week 1 - day 1
### VM-Setup Network

1. Ubah adapter ke mode Bridge agar mendapatkan IP dari jaringan yang sama. Klik kanan pada logo yang ditandai warna merah, lalu klik network setting.
    
    ![networkSetting](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Setup%20Network/img/1.png)

2. Ubah NAT adapter ke Bridge Adapter, lalu pilih tipe perangkat yang terkoneksi ke jaringan. Pada kali ini dipilih Wi-fi.
    
    ![Bridge](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Setup%20Network/img/2.PNG)

3. Cek gateway pada jaringan.
    
    ![GW](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Setup%20Network/img/3.PNG)

4. Edit file konfigurasi network.
    
    ![conf-network](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Setup%20Network/img/4.PNG)

5. Ubah agar menjadi IP static. DHCP diubah menjadi "no", lalu masukan addresses, gateway, dan nameservers
    
    ![staticIP](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Setup%20Network/img/5.PNG)

6. Apply perubahan IP yang dilakukan.
    
    ![apply](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Setup%20Network/img/6.PNG)

7. Apabila tidak ada error, bisa langsung coba ping ke internet. Apabila ada error pastikan file config network sudah sesuai.
    
    ![Ping](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/VMWare-Setup%20Network/img/7.PNG)
