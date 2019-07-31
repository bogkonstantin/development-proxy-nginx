# Setup for testing local development  
For example you can use it to test WebHooks on local server.  
  
## Prerequisites  
* docker  
* docker-compose  
  
## Configuration  
Default port - 8080. Change it in docker-compose.yml if you need.  
Default proxy url is mylocalwebsite.domain. Change it to your domain.  
  
## Running  
After configuration, start container:  
```
docker-compose up -d
```
  
And start tunnel:  
```
ssh -R 80:localhost:8080 serveo.net
```   

Read more about https://serveo.net/