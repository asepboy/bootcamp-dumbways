# Dumbways Bootcamp DevOps
## Week 4
### Connect Multiple Server to Prometheus

### Setup Grafana

1. Lakukan login pada grafana
   
   ![1](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/1.png)

2. Lalu tambahkan data source prometheus
   
   ![4](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/4.png)

   ![5](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/5.png)

3. Lalu setup prometheus pada web grafana. Dengan menambahkan URL dari prometheus. pastikan tidak terdapat warning atau failed.
   
   ![6](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/6.png)

4. Selanjutnya membuat dashboard untuk monitoring, dengan mengklik "Create", lalu "Add Panel". 
   
   ![7](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/7.png)

   ![8](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/8.png)

5. Selanjutnya pada query pilih prometheus, dan pada metrics masukan metrics apa yang akan di monitor. metrics ini dapat diambil dari web prometheus. 
   
   ![9](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/9.png)

6. Dan pada gambar dibawah sudah diperlihatkan kondisi server yang dimonitoring.
   
   ![10](/week4/ConnectMultipleServertoPrometheus/img/SetupGrafana/10.png)


