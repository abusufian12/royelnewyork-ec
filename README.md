# royelnewyork-ec

PHP version need: php 7.4

yarn dev:shop-rest

yarn dev:admin-rest

// add IP if add server ip on next.config.js file

// create .babelrc file on shop and other nextjs project directory and put in .babelrc file: { "presets": ["next/babel"] }

yarn build:shop-rest

// build:rest for production

// for laravel

composer install

PHP plugins you must need

simplexml PHP's dom extension mbstring GD Library

php artisan marvel:install

if change APP_URL=http://localhost:8000 in laravel env file then need to storage:link and run command again
sudo rm storage // from public folder

php artisan storage:link

php artisan serve

sudo chown -R www-data:www-data public/storage

sudo chown -R $USER:www-data public/storage

sudo chmod -R 777 public/storage

sudo chmod -R 777 bootstrap/cache

//admin /// SQLSTATE[23000]: Integrity constraint violation: 1062 Duplicate entry 'en' for key 'settings_language_unique' (SQL: insert into settings Then in at settings table in language column have unique key. so need to chnage language or pass different language name


under .next folder cache folder should be delete before push to git 

if not running frontend alwyes check pm2 status 



How to rebuild shop?
When you upload the code to the server as a production, NextJS fetch its code from the build file. So after deployed, when you update or change code on scripts, the updated scripts don't work at admin end until you rebuild the project again. NextJs works this way.

Now there are two ways you can follow to rebuild shop,

If your server has more than 2+ CPU core and 6GB+ of memory, then you can directly edit code at your server then rebuild the project from the server directly using this command,

For shop,

Go to /var/www/pickbazar-laravel/shop

yarn build
After completing the build, restart the PM2 process using this command,

pm2 restart 'all'


But suppose your server doesn't have that processing power, and you try to build your scripts directly from the server. In that case, your server will be shut down during the build, and you've to restart the server.


