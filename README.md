# annotations-cheatsheet

# Spring, Spring Boot Annotations Cheat sheet

### Spring Boot Main annotations 
- @SpringBootApplication
  - Contains: 
  - @ComponentScan - scan your beans -> visible to ioc container
  - @EanbleAutoConfiguration - automatically configures the spring application based on jar dependency that we have added in our         pom.xml 
      e.g. h2database jar is present in class path & we have not configured any beans related to the database manually -> it'll           configure it manually 
  - @Configuration - define the bin definitions inside this class -> spring IOC can load it

### Stereotype annotation - used to create spring beans automatically in ApplicationContext & Spring will manage its lifecycle
- @Component: 
  - Below are all derived from component class: 
  - @Controller - web layer where we can expose our rest api
  - @Service - write business logic
  - @Repository - write database logic
  - ^ annotate differently -> tell role of that class
