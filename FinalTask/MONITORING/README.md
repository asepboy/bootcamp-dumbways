# Dumbways Bootcamp DevOps
## Final Task

### Monitoring

1. Clone Repo dari Github untuk monitoring. Sama seperti sebelumnya saya sudah pernah mengkonfigurasi dan disimpan di github. Namun pada repo ini hanya untuk master, sehingga untuk slave yang hanya menginstall node exporter dilakukan tanpa bantuan ansible ataupun docker. Pada file konfigurasi prometheus.yml dikonfigurasi agar dapat mnerima pull metrics dari tiap server slave.
   
   ![1](/FinalTask/MONITORING/IMG/1.png)

   ![2](/FinalTask/MONITORING/IMG/2.png)

   ![12](/FinalTask/MONITORING/IMG/12.png)

2. Jalankan file docker compose.
   
   ![3](/FinalTask/MONITORING/IMG/3.png)

   ![4](/FinalTask/MONITORING/IMG/4.png)

3. Setelah itu akses domain untuk prometheus dan grafana
   
   ![5](/FinalTask/MONITORING/IMG/5.png)

   ![6](/FinalTask/MONITORING/IMG/6.png)

4. Pada grafana tambahkan data source untuk prometheus.
   
   ![6](/FinalTask/MONITORING/IMG/6.png)

5. Lalu tambahkan panel untuk percobaan.
   
   ![7](/FinalTask/MONITORING/IMG/7.png)

6. Gambar dibawah contoh untuk menampilkan dashboard storage yang digunakan.
   
   ![8](/FinalTask/MONITORING/IMG/8.png)

   ![9](/FinalTask/MONITORING/IMG/9.png)

   ![10](/FinalTask/MONITORING/IMG/10.png)

7. Gambar dibawah menampilkan detail dari setiap server yang dimonitor, dengan menggunakan template.
   
   ![11](/FinalTask/MONITORING/IMG/11.png)
