# Docker configuration for WordPress

## Prerequires

You'll need to install Docker and Docker Compose on your local machine.


## Set up

- Clone the project 

```bash
git clone https://github.com/alexeisersun/wp-bestch-site.git
```

- Change your working directory to 

```bash
cd wp-bestch-site
```

- Copy `docker-compose.example.yml` to `docker-compose.yml`

```bash
cp docker-compose.example.yml docker-compose.yml
```

- In `docker-compose.yml` change `WORDPRESS_DB_USER`, `WORDPRESS_DB_PASSWORD` and `WORDPRESS_DB_NAME` for both `wordpress` and `db` services to custom values. Set _secure_ password.

- Run `docker-compose up`.

- Open `localhost:8080` in your favorite browser. You'll be redirected to `/wp-admin/install.php` where you'll be prompted to add information about your admin account. Set _secure_ password.
