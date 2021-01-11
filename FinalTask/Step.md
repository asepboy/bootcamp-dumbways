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

3. Lalu isi file seperti gambar dibawah
   ```yml
   public ansible_python_interpreter=/usr/bin/python3
    database ansible_python_interpreter=/usr/bin/python3
    jenkins ansible_python_interpreter=/usr/bin/python3
    monitoring ansible_python_interpreter=/usr/bin/python3
    frontend ansible_python_interpreter=/usr/bin/python3
    backend ansible_python_interpreter=/usr/bin/python3

    public ansible_host=172.16.1.147 ansible_user=gilbranpublic
    database ansible_host=172.16.2.49 ansible_user=gilbrandatabase
    jenkins ansible_host=172.16.2.107 ansible_user=gilbranjenkins
    monitoring ansible_host=172.16.2.10 ansible_user=gilbranmonitoring
    frontend ansible_host=172.16.2.46 ansible_user=gilbranfrontend
    backend ansible_host=172.16.2.108 ansible_user=gilbranbackend

    [nginx]
    public

    [mysql]
    database

    [docker]
    jenkins
    monitoring
    frontend
    backend
   ```