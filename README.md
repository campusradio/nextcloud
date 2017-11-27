# nextcloud
File Server


## Getting Started

```bash
# Clone
git clone https://github.com/campusradio/nextcloud.git

# Put own password, user & dbname inside the .env file
cp sample.env .env
vim .env

# Let's docker
docker-compose up -d
```

## Volumes

Conains all the necessary volumes for persistence, so can be updated without issues.

###### Nextcloud Server

- ./data/nc/data:/var/www/html/data
- ./data/nc/config:/var/www/html/config
 - ./data/nc/custom_apps:/var/www/html/custom_apps
 - ./data/nc/themes:/var/www/html/themes

###### Postgres

- ./data/db:/var/lib/postgresql/data
