# Dumbways Bootcamp DevOps
## Week 2
### Custom Domain for Backend Application


1. Pada dashboard cloudflare, tambahkan subdomain dengan name "api.gilbran" dan IPv4 Address dengan IP Public dari Public instance, dan rubah proxy status menjadi DNS.
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/CustomDomainforBackendApplication/img/1.png)

2. Lalu pada file reverse proxy backend, ubah server name menjadi domain yang baru.
   
   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/CustomDomainforBackendApplication/img/2.png)

3. Pada server frontend edit file /src/config/api.js dengan merubah baseURL dengan mengganti IP menjadi domain baru.
   
   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/CustomDomainforBackendApplication/img/3.png)

4. Coba akses domain baru pada browser.
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/CustomDomainforBackendApplication/img/4.png)