# dockerize-spring-boot


1. add docker-maven-plugin (+  modify <baseImage>java:8</baseImage>, <imageName>dockerdemo</imageName> -> must be lowercase.. )
2. mvn clean install
3. mvn docker:buld -> create /target/docker folder with Dockerfile

4. docker images (should see dockerdemo and java images)
5. docker run -p 9999:8080 dockerdemo

6. alebo nepouzit docker:build z mavenu, ale zbuildovat rucne cez: docker build -f Dockerfile -t docker-spring-boot . (bodka na konci je dolezita)

