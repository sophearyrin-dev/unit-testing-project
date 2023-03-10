# 1. Unit testing
Unit Testing is a one of the testing done by the developers to make sure individual unit or component functionalities are working fine.

## Annotation
- @Profile(“test”) annotation is used to configure the class when the Test cases are running.
- Spring Profiles provide a way to segregate parts of your application configuration and make it only available in certain environments. 
Any @Component or @Configuration can be marked with @Profile to limit when it is loaded:
```
@Configuration
@Profile("production")
public class ProductionConfiguration {

    // ...

}
- A bean is an object that is instantiated, assembled, and otherwise managed by a Spring IoC container.

```
- @Before annotation are run before each test. This is useful when we want to execute some common code before running a test

## Method
- The assertThat is one of the JUnit methods from the Assert object that can be used to check if a specific value match to an expected one.
- To capture the method arguments, you need to use the capture() method of ArgumentCaptor. You should call it during the verification phase of the test.
## Mockito
Mockito
For injecting Mockito Mocks into Spring Beans, we need to add the Mockito-core dependency in our build configuration file.
```
<dependency>
   <groupId>org.mockito</groupId>
   <artifactId>mockito-core</artifactId>
   <version>2.13.0</version>
</dependency>
<dependency>
   <groupId>org.springframework.boot</groupId>
   <artifactId>spring-boot-starter-test</artifactId>
   <scope>test</scope>
</dependency>
```
