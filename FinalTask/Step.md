# DevOps Final Task
## Step by Step

### Schematic

Schematic yang digunakan

![schematic](/FinalTask/img/schematic/FinalTask.png)

### Seluruh Server
Siapkan server sesuai kebutuhan.
Buat NAT, agar semua dapat terkoneksi ke internet.
Buat file authorized_keys di directory ```.ssh/``` disetiap server, lalu paste id_rsa.pub dari server public dan server ansible ke authorized_keys disetiap server.
Lalu pastikan server dapat diremote dari server ansible.

### Server Ansible
1. Lakukan update dan upgrade, lalu install ansible.
   ```apt update && apt upgrade -y```
   
   ```apt install ansible -y ```

2. Buat file ```Inventory``` di ```~/ansible/```. Folder dibuat baru.

   ``` 
   mkdir ansible
   cd ansible
   sudo nano Inventory
   ```

3. Lalu clone link dibawah
   [git@github.com:gilbranfairuz/ansiblePlaybook.git](git@github.com:gilbranfairuz/ansiblePlaybook.git)