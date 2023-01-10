# full-liferay-docker
This repo is example for complete Liferay 7.4 platform with MySQL and ES using Docker

## build project

Make sure that you setup Java JDK 11 on classpath, then run
```
./gradlew buildDockerImage
```
to build docker image of Liferay Portal CE 7.4 locally.

## run project
To run project, we need to run previous built image with port mapping and environment variables.
```
docker run -it -m 4g -p 8080:8080 -e JAVA_VERSION=zulu11 --name=liferay-portal-7.4 liferay/portal:7.4.3.57-ga57
```
Go to http://localhost:8080 to see Liferay Portal CE 7.4. 

Click on "Sign In" to see the login page. 
Username is "test@liferay.com" and password is "test". 
Update username and password and you are good to go. :)

