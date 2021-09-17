cd src 
composer install
npm install 
npm run dev
cd ..
chmod -R 777 ./src/storage
docker
docker-compose up -d --build



sudo docker-compose exec php php /var/www/html/artisan migrate
 sudo docker-compose exec php php /var/www/html/artisan db:seed
