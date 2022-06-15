Laravel v9.11.0 (PHP v8.0.2), Nginx:alpine, mysql:5.7.22

### Installation

Rename "laravel/.env.example" to ".env"<br><br>
<code>$ composer install</code><br><br>
<code>$ docker-compose up -d</code><br><br>
<code>$ docker-compose exec app php artisan key:generate</code><br><br>
<code>$ docker-compose exec app php artisan config:cache</code><br><br>
<code>$ docker-compose exec app php artisan migrate</code><br><br>

### Configuration 
php.ini
<code>/php/local.ini</code>

mysql
<code>/mysql/my.cnf</code>

nginx
<code>/nginx/conf.d/app.cnf</code>

### Commands

Estructure<br>
<code>$ docker-compose exec "service" "command"</code>

example<br>
<code>$ docker-compose exec app php artisan make:controller UserController</code><br><br>
<code>$ docker-compose exec db bash</code>
