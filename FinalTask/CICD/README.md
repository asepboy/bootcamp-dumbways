# Dumbways Bootcamp DevOps
## Final Task

### CI/CD

1. Clone repo untuk jenkins dari github. Sebelumnya saya pernah menggunakan jenkins, sehingga pada kegiatan ini dapat menggunakan docker-compose yang sama.
   
   ![1](/FinalTask/CICD/IMG/1.png)

2. Jalankan playbook tersebut.
   
   ![2](/FinalTask/CICD/IMG/2.png)
   
3. Setelah clone, pada docker-compose.yml tambahkan volume.
   
   ![3](/FinalTask/CICD/IMG/3.png)

4. Karena sebelumnya sudah dikonfigurasi untuk domain sehingga tidak diperlihatkan proses Reverse proxy, custom domain dan SSL. Akses domain jenkins. Lalu cek password pada direktori yang diperlihatkan di browser.
   
   ![4](/FinalTask/CICD/IMG/4.png)

5. Install Plugins
   
   ![5](/FinalTask/CICD/IMG/5.png)

6. Instance Configuration dimasukan domain dari cicd.gilbran.instructype.com
   
   ![8](/FinalTask/CICD/IMG/8.png)

7. Setelah selesai lakukan Login.
   
   ![10](/FinalTask/CICD/IMG/10.png)

8. Lakukan install plugin publish over SSH. Agar jenkins dapat melakukan remote melalui SSH ke server yang berangkutan (Backend, Frontend).
   
9.  Selanjutnya manage credential untuk server yang akan melakukan remote. Klk manage credential, lalu klik Jenkins, yang diberi highlight merah.
   
   ![11](/FinalTask/CICD/IMG/11.png)

   ![12](/FinalTask/CICD/IMG/12.png)

11. Lalu klik Global Credential, dan tambahkan credential.
    
    ![13](/FinalTask/CICD/IMG/13.png)

    ![14](/FinalTask/CICD/IMG/14.png)

12. Karena remote menggunakan SSH, pilih SSH username and key. Lalu field sesuai ketentuan yang diperlukan.
    
    ![15](/FinalTask/CICD/IMG/15.png)

13. Selanjutnya, kembali ke dashboard dan klik configure system. 
    
    ![16](/FinalTask/CICD/IMG/16.png)

14. Pada bagian Publish over SSH (paling bawah), berikan informasi mengenai server mana saja yang akan di remote oleh Jenkins. Dalam kegiatan ini hanya backend dan frontend yang akan diremote oleh Jenkins.
    
    ![17](/FinalTask/CICD/IMG/17.png)

    ![18](/FinalTask/CICD/IMG/18.png)

15. Setelah selesai memberikan informasi mengenai server yang diremote, sekarang menambahkan job untuk frontend dan backend. Job type yang dipilih adalah freestyle.
    
    ![19](/FinalTask/CICD/IMG/19.png)

    ![20](/FinalTask/CICD/IMG/20.png)
    
16. Setelah membuat nama job yang akan dikerjakan, pada "source code management" tambahkan link repo git dari masing masing project (backend dan frontend), tentukan credential, dan juga branch yang digunakan.
    
    ![21](/FinalTask/CICD/IMG/21.png)

17. Pada build trigger pilih Github hook trigger, agar git menjadi indikator apabila ada perubahan dari developer.
    
    ![22](/FinalTask/CICD/IMG/22.png)

18. Pada field "Build" adalah proses build yang diakan dilakukan oleh Jenkins ke server remote, pada field ini dimasukan apa saja yang akan dilakukan oleh server tersebut melalui jenkins. Source file diisi dengan "/", lalu remote directory diisi "home/user", dan pada exec command diberikan command yang akan dilakukan, mulai dari pindah directory, melakukan pull dari repo, mematikan docker yang sedang berjalan, dan menghapus docker yang terakhir, melakukan build image, lalu melakukan docker-compose up. 
    
    ![23](/FinalTask/CICD/IMG/23.png)

19. Untuk job selanjutnya step yang dilakukan sama, sehingga hanya diperlihatkan gambarnya saja.
    
    ![24](/FinalTask/CICD/IMG/24.png)

    ![25](/FinalTask/CICD/IMG/25.png)

    ![26](/FinalTask/CICD/IMG/26.png)

20. Menghubungkan webhook jenkins ke github. Hal ini dilakukan agar apabila ada perubahan dari developer yang di push ke github, maka jenkins akan langsung melakukan perubahan pada server yang bersangkutan. Dan juga dari github akan dihubungkan ke hub docker, sehingga akan langsung dibuat image. Pada setting repo klik webhooks, lalu tambahkan domain dari jenkins ditambah /github-webhook/ (plugin webhook github) (cicd.gilbran.instructype.com/github-webhook/).
    
    ![27](/FinalTask/CICD/IMG/27.png)

    ![28](/FinalTask/CICD/IMG/28.png)

21. Untuk terhubung ke docker hub, tambahkan link account pada tiap image ke github, lalu pada menu builds ubah source ke branch yang digunakan (production). Setelah selesai dikonfigurasi, tampilannya akan seperti dibawah.
    
    ![29](/FinalTask/CICD/IMG/29.png)

    ![30](/FinalTask/CICD/IMG/30.png)

22. Selanjutnya untuk tambahan, akan diberikan notifikasi email apabila ada build yang dilakukan oleh jenkins. 
23. Pada configuration, field Extended E-mail Notification diisi sesuai dengan kebutuhan. Dan pastikan email yang akan digunakan untuk mengirim notifikasi diberi akses untuk third party apps, seperti dibawah.
    
    ![34](/FinalTask/CICD/IMG/34.png)

    ![35](/FinalTask/CICD/IMG/35.png)

    ![32](/FinalTask/CICD/IMG/32.png)

    ![33](/FinalTask/CICD/IMG/33.png)

24. Lalu pada setiap job, pada menu post-build action pilih editable email notification. 
    
    ![36](/FinalTask/CICD/IMG/36.png)

25. Pilih trigger always, agar setiap ada build baik failure, unstable, success ataupun yang lainnnya akan diberikan notifikasi email oleh jenkins. Dan pada log klik attach build log, agar lognya dikirimkan juga melalui email.
    
    ![37](/FinalTask/CICD/IMG/37.png)

    ![38](/FinalTask/CICD/IMG/38.png)

    ![39](/FinalTask/CICD/IMG/39.png)

26. Berikut adalah contoh build success
    
    ![40](/FinalTask/CICD/IMG/40.png)

    ![41](/FinalTask/CICD/IMG/41.png)

27. Berikut adalah contoh build unstable
    
    ![42](/FinalTask/CICD/IMG/42.png)

    ![43](/FinalTask/CICD/IMG/43.png)