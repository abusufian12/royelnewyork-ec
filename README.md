# royelnewyork-ec

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
