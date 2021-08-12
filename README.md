# LaravelAuth

Laravel

## Setup

### Clone

```sh
git clone https://github.com/okazakikyo/LaravelAuth
cd LaravelAuth
cp .env.example .env
composer install
```

### Generate a Laravel Application key

```
php artisan key:generate
```

### Setup the database

Create a `laravelcustom` database:

```sql
CREATE DATABASE IF NOT EXISTS `laravelcustom`;
```

Modify the `laravelcustom/.env` file and set the following:

```
APP_NAME="LaravelAuth"

DB_HOST=<mysql_server_address>
DB_DATABASE=laravelcustom
DB_USERNAME=<mysql_username_eg_root>
DB_PASSWORD=<mysql_password_eg_root>
```


Run Laravel migrations:
```sh
php artisan migrate
```


### Compile the frontend part

```sh
npm install
npm run dev
```

While developing, you can use:

```sh
npm run watch
```


