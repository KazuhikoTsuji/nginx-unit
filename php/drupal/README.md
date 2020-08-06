curl --output ./drupal-8.6.4.tar.gz https://ftp.drupal.org/files/projects/drupal-8.6.4.tar.gz
tar xvzf ./drupal-8.6.4.tar.gz
docker build -t nginxunit-php:drupal-8.6.4 .
docker run -d --name drupal-8.6.4 -p 80:80 nginxunit-php:drupal-8.6.4