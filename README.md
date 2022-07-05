# Springboot dockerized app

## First version
1. Installed Java, Maven, Intellij  


2. Installed Docker Desktop (Account in docker hub) - Docker Runtime Engine


3. Create springboot application


4. Import to Intellij


5. Create REST Endpoint


6. Create Dockerfile


7. Create docker image  
   docker build -t application-one-img .


8. Push docker image to docker hub repository  
   create image to push: ```docker tag application-one-img carlonicolo/application-one-img```docker,  
   create image with tag and version to push: ```docker tag application-one-img:latest carlonicolo/application-one-img:v1```docker,    
   push image to docker hub with no version it takes latest version: ```docker push carlonicolo/application-one-img```docker,    
   push image to docker hub: ```docker push carlonicolo/application-one-img:v1```docker,  


9. Pull docker image from docker hub repository  
   pull image from docker hub: docker run -p 8090:8080 carlonicolo/application-one-img:latest


10. Run the pulled docker image in our local computer


11. Run multiple containers  
    docker ps run ps 8091:8080 carlonicolo/application-one-img:latest