# Spring boot
## Running spring boot app with Intellij Idea

This is kind of 'HelloWorld' sample with simple tips to perform spring boot application.

**Table of Contents**

__TOC__

### Setup environment

- [Java Development Kit](https://www.oracle.com/technetwork/java/javase/downloads/)
- [Intellij Idea Ultimate](https://www.jetbrains.com/idea/download/)
- [MySQL](https://dev.mysql.com/doc/mysql-getting-started/en/#mysql-getting-started-installing) (or any other DB you prefer)

### Create simple app 

Run  IDEA

- New -> Project... -> Spring Initializr

![](https://miro.medium.com/max/1200/1*DaNjDrcwZ0uzRYU3kyaZdg.png)

press [Next]

- Fill [GroupId, ArtifactId, Version](https://maven.apache.org/guides/mini/guide-naming-conventions.html) and other fields
- [Next] -> . . . -> [Next] ->  . . . -> [Finish]

Run the app:
> Process finished with exit code 0


### Prepare project structure

	├── ...
	├── src
	│   ├── main
	│   │    └── java
	│   │          ├── controllers         # to be added
	│   │          ├── entities            # 
	│   │          ├── services            # 
	│   │          ├── repositories        #
	│   │          └── Application.java
	│   └── resources
	│        └── application.properties
	├── pom.xml
	└── ...
	
### Spring Data + Hibernate
Add following dependecies to POM file:

```xml
<dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-data-jpa</artifactId>
        <version>2.1.6.RELEASE</version>
</dependency>

```
