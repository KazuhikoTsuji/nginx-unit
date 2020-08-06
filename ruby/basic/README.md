docker build -t nginxunit-ruby:basic .  
docker run -d --name nginxunit-ruby -p 8080:8080 nginxunit-ruby:basic  