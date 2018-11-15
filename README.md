
# Jenkins Setup for Enonic Cloud
Jenkins server with apache2 and letsencrypt SSL certificates included.

## Configuration
### docker-compose.yml
Update:
- hostname on all containers
- LETS_ENCRYPT_EMAIL and LETS_ENCRYPT_DOMAIN in apache2/environment
- ServerName in apache2/sites/0-default.conf
- Lets Encrypt requires that the server is reachable on the domain you specify instead of yourdomain.com
## Installation
```
docker-compose build
docker-compose up -d
```
