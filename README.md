# spring-boot-logging demo


## 1)Default Logging Setup
By default, Spring Boot:

<ul><li>Uses Logback as the underlying logging framework.</li><br>
<li>Logs output to the console.</li><br>
<li>Supports logging levels: TRACE, DEBUG, INFO, WARN, ERROR, and FATAL.</li></ul>

 ### Technical Details
In this project, we are going to use below set of versions for demonstrations.

    Spring Boot - 3.3.3
    Spring - 6.1.12
    Lombok - 1.18.34
    jdk-17

### Building

The example can be built with
```shell
mvn clean install
```

### Running the example in your local
```shell
mvn clean spring-boot:run
```
## dependency
```shell
<dependency>
      <groupId>io.micrometer</groupId>
     <artifactId>micrometer-core</artifactId>
</dependency>
<dependency>
    <groupId>io.micrometer</groupId>
    <artifactId>micrometer-registry-prometheus</artifactId>
<scope>runtime</scope>
</dependency>
```
# log link
```shell
http://localhost:8089/log
```
# actuator link
```shell
http://localhost:8089/actuator
```
## Logger
-->Copy this project to your local machine<br>
-->Build thi project using mvn clean install -DskipTests command<br>
-->Run this application as java application or execute mvn spring-boot:run command<br>
-->This application is demo for logger; we can understand how logger works<br>
-->Once application started, please check the logs.<br>
-->Open http://localhost:8088 in browser, you will see Greeting demo page. Put your name and get greetings.<br>
-->Now, open http://localhost:8089/log in browser. Check the message and logs.<br>
-->Now, openhttp://localhost:8089/actuator in browser. Check the message and logs.<br>
-->Please change the log level configuration in the application.properties for logging.level.root and re-run. You will find the difference of log level.
