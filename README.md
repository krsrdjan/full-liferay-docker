# full-liferay-docker
Example for complete Liferay 7.4 platform with MySQL and ES using Docker.

## build project

Make sure that you setup Java JDK 11 on classpath and Docker and docker-compose installed.
Run this command
```bash
./gradlew buildDockerImage
```
to build docker image of Liferay Portal CE 7.4 locally. 
This image will be used in docker-compose.yml

## run project
To run project, you need to have Docker and docker-compose installed.
Go to docker folder in project root and run
```bash
cd docker
docker-compose up -d
```
Wait for a while until all containers are up and running. Check Liferay container logs until you see
"Server startup in [xxx] ms message". 

Then you can access Liferay Portal at http://localhost:8080

Click on "Sign In" to get login page. 

Username is "test@liferay.com" and password is "test". 

Update password, so you are good to go. :)

