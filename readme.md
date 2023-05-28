# NGINX Proxy Manager

visit manager.londonparkour.com
Links:
- https://www.nikitakazakov.com/nginx-proxy-manager-docker-multiple-sites
- https://web.vnappmob.com/page/hosting-multiple-sites-or-applications-using-docker-and-nginx-reverse-proxy-with-letsencrypt-ssl-139






## Issues

### 504 Gateway Timeout

When trying to setup manager.londonparkour.com proxy subdomain the url kept going to a 504. I had to assign a reserved IP within digitalocean for it to work.


### Failing to start

The default demo docker-compose file has a volume `./data` for the app and `./data/mysql` for the database. The app needs to be put into a separate folder `./data/app` and `./data/mysql`.

