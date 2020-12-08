# Dumbways Bootcamp DevOps
## Week 1
### VM-Setup Network

1. Ubah adapter ke mode Bridge agar mendapatkan IP dari jaringan yang sama. Klik kanan pada logo yang ditandai warna merah, lalu klik network setting.
    
    ![networkSetting]()

2. Ubah NAT adapter ke Bridge Adapter, lalu pilih tipe perangkat yang terkoneksi ke jaringan. Pada kali ini dipilih Wi-fi.
    
    ![Bridge]()

3. Cek gateway pada jaringan.
    
    ![GW]()

4. Edit file konfigurasi network.
    
    ![conf-network]()

5. Ubah agar menjadi IP static. DHCP diubah menjadi "no", lalu masukan addresses, gateway, dan nameservers
    
    ![staticIP]()

6. Apply perubahan IP yang dilakukan.
    
    ![apply]()

7. Apabila tidak ada error, bisa langsung coba ping ke internet. Apabila ada error pastikan file config network sudah sesuai.
    
    ![Ping]()

