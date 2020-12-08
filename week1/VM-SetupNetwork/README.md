# Dumbways Bootcamp DevOps
## Week 1
### VM-Setup Network

1. Ubah adapter ke mode Bridge agar mendapatkan IP dari jaringan yang sama. Klik kanan pada logo yang ditandai warna merah, lalu klik network setting.
    
    ![networkSetting](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-SetupNetwork/img/1-1.png)

2. Ubah NAT adapter ke Bridge Adapter, lalu pilih tipe perangkat yang terkoneksi ke jaringan. Pada kali ini dipilih Wi-fi.
    
    ![Bridge](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-SetupNetwork/img/1-2.png)

3. Cek gateway pada jaringan.
    
    ![GW](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-SetupNetwork/img/1-3-cekGW.png)

4. Edit file konfigurasi network.
    
    ![conf-network](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-SetupNetwork/img/1-4.png)

5. Ubah agar menjadi IP static. DHCP diubah menjadi "no", lalu masukan addresses, gateway, dan nameservers
    
    ![staticIP](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-SetupNetwork/img/1-5.png)

6. Apply perubahan IP yang dilakukan.
    
    ![apply](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-SetupNetwork/img/1-6.png)

7. Apabila tidak ada error, bisa langsung coba ping ke internet. Apabila ada error pastikan file config network sudah sesuai.
    
    ![Ping](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/VM-SetupNetwork/img/1-7.png)

