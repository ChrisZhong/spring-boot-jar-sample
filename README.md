spring-boot-jar-sample
======================
**Continuous Integration**: [![Build Status](https://travis-ci.org/ChrisZhong/spring-boot-jar-sample.svg?branch=master)](https://travis-ci.org/ChrisZhong/spring-boot-jar-sample)

##Instructions
This is a spring-boot example that builds an executable jar file for loading externally located application.properties file by using the environment variables.

1. The sample application.properties file is located in the root of this project. You can move it to whatever location you desire.
2. If the environment variable, `SPRING_CONFIG_LOCATION`, does not exist, create it and point it to the location of the properties file. For example, if your system is Linux and the properties file is located in `/etc/`, then `SPRING_CONFIG_LOCATION = /etc/`. If your machine is Windows and the properties file is located in the root of your user directory, then `SPRING_CONFIG_LOCATION = %UserProfile%`.
3. Build your application `gradlew build` and run the application using `java -jar spring-boot-jar-sample.jar`.
4. Open up your favorite browser and browse to `localhost:8080`. If you see a message starting with "Hello World!" and the values from the properties file. Then it works correctly.
