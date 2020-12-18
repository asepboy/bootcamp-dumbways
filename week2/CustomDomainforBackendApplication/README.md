# Dumbways Bootcamp DevOps
## Week 2
### Custom Domain for Backend Application


1. Pada dashboard cloudflare, tambahkan subdomain dengan name "api.gilbran" dan IPv4 Address dengan IP Public dari Public instance, dan rubah proxy status menjadi DNS.
   
   ![1]()

2. Lalu pada file reverse proxy backend, ubah server name menjadi domain yang baru.
   
   ![2]()

3. Pada server frontend edit file /src/config/api.js dengan merubah baseURl dengan mengganti IP menjadi domain baru.
   
   ![3]()

4. Coba akses domain baru pada browser.
   
   ![4]()