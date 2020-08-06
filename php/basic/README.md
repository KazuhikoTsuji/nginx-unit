docker build -t nginxunit-php:basic .  
docker run -d --name nginxunit-php -p 8080:8080 nginxunit-php:basic  