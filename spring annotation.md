
# 50+ Spring Boot Most Important Annotations

## 🌟 Exciting Spring Boot Annotations for Building Powerful Applications! 🌟

Hey GitHub fam! 👋 Today, I want to share with you some essential Spring Boot annotations that can supercharge your development process. These annotations make it easier to build robust and efficient applications. Let's dive in!


## 🚀 Spring Boot Main Annotations 🚀

1️⃣ @SpringBootApplication: This is the starting point of any Spring Boot application. It combines three annotations - @Configuration, @EnableAutoConfiguration, and @ComponentScan. It sets up the application, enables auto-configuration, and scans for components.

2️⃣ @ComponentScan: This annotation tells Spring where to look for components, such as controllers, services, and repositories. It helps Spring find and register these components automatically.

3️⃣ @EnableAutoConfiguration: This annotation enables Spring Boot's auto-configuration feature, which automatically configures the application based on the dependencies present in the classpath. It saves you from writing boilerplate configuration code.

4️⃣ @Configuration: This annotation identifies a class as a configuration class. It declares and wires beans that can be used by the application. It's a key building block for creating custom configurations.



## 💡 Stereotype Annotations 💡

1️⃣ @Component: This annotation marks a class as a Spring-managed component. It's a generic stereotype for any Spring-managed component.4

2️⃣ @Service: This annotation represents a service layer component. It's used to define business logic and perform service-oriented tasks.

3️⃣ @RestController / @Controller: These annotations are used to define controller classes that handle incoming HTTP requests. @RestController is a combination of @Controller and @ResponseBody, making it ideal for building RESTful APIs.

4️⃣ @Repository: This annotation is used to identify a class as a data access object (DAO) or repository. It enables Spring to perform database operations easily.


## 🌱 Spring Core Annotations (Continued) 🌱

1️⃣ @Bean: This annotation is used inside a configuration class to define a bean. A bean represents an object that Spring manages and injects into other parts of the application.

2️⃣ @Autowired: With this annotation, you can automatically inject dependencies into your beans. It helps to wire different parts of your application together effortlessly.

3️⃣ @Qualifier: When multiple beans of the same type exist, @Qualifier helps in selecting the correct bean to be injected.
4️⃣ @Lazy: This annotation tells Spring to create a bean only when it's needed, not during the application startup. It can save resources if the bean is not always used.

5️⃣ @Value: It is used to inject values from properties files or environment variables into Spring beans.

6️⃣ @PropertySource: This annotation allows you to specify the properties file from which the @Value annotation will read the values.

7️⃣ @ConfigurationProperties: It binds external configuration properties to fields of a Java bean.

8️⃣ @Profile: With this annotation, you can define beans that will be activated based on specific profiles. It helps in managing different configurations for different environments.

9️⃣ @Scope: This annotation allows you to specify the scope of a Spring bean (singleton, prototype, etc.). It defines how many instances of a bean should exist.


## 🌐 REST API Annotations 🌐

These annotations are crucial for building RESTful APIs in Spring Boot.
1️⃣ @RestController: As we mentioned earlier, this annotation combines @Controller and @ResponseBody. It's used to create RESTful web services that directly return data in the response body.

2️⃣ @RequestMapping: This annotation maps HTTP requests to specific controller methods based on the URL pattern.

3️⃣ @GetMapping, @PostMapping, @PutMapping, @DeleteMapping: These annotations specify the HTTP methods (GET, POST, PUT, DELETE) that a controller method can handle.

4️⃣ @RequestBody: It's used to extract the request body and convert it into a Java object for processing.

5️⃣ @PathVariable: This annotation binds the URL template variables to the method parameters.

6️⃣ @RequestParam: It binds query parameters from the URL to the method parameters.

7️⃣ @ControllerAdvice & @ExceptionHandler: These annotations are used for global exception handling in Spring MVC applications. They help to handle exceptions across all controllers.

## 📚 Spring Data JPA Annotations 📚

These annotations simplify working with relational databases using JPA (Java Persistence API).
1️⃣ @Entity: This annotation marks a class as an entity, representing a table in the database.

2️⃣ @Table: It is used to specify the table name associated with the entity.

3️⃣ @Column: This annotation maps a class field to a database column.

4️⃣ @Transactional: This annotation defines a transactional method or class. It ensures that the method is executed within a transaction.

5️⃣ Entity class relationships: @OneToOne, @OneToMany, @ManyToOne, @ManyToMany: These annotations define relationships between entities, such as one-to-one, one-to-many, many-to-one, and many-to-many.

## 📚Spring Security Annotations📚

1️⃣@EnableWebSecurity: This annotation enables the Spring Security configuration for securing web applications.

2️⃣@Secured: It is used to apply method-level security to controllers or service methods.

3️⃣@PreAuthorize / @PostAuthorize: These annotations define pre- or post-authorization expressions to restrict access to methods based on specific conditions.

4️⃣@AuthenticationPrincipal: It allows you to access the currently authenticated user principal within a controller or service.

## 🌟Spring Caching Annotations🌟

1️⃣@EnableCaching: This annotation enables Spring's caching infrastructure for caching method results.

2️⃣@Cacheable: It indicates that the result of a method should be cached. Subsequent calls with the same parameters will be retrieved from the cache instead of executing the method.

3️⃣@CacheEvict: This annotation is used to remove specific entries or clear the entire cache.

4️⃣@CachePut: It updates the cache with the result of a method, regardless of whether the cache already contains a value for the given key.

## 🌟Spring AOP (Aspect-Oriented Programming) Annotation🌟

1️⃣@Aspect: This annotation defines a class as an aspect, which encapsulates cross-cutting concerns.

2️⃣@Pointcut: It specifies a set of join points (methods) where an advice (aspect) should be applied.

3️⃣@Before, @After, @AfterReturning, @AfterThrowing: These annotations specify different types of advice that should be executed before, after, or around a method invocation.

4️⃣@Around: It allows you to wrap the advised method with custom code, controlling the entire method invocation.

## 🌱Spring Validation Annotations🌱

1️⃣@Valid: This annotation is used to validate the annotated object or method parameter.

2️⃣@NotNull, @NotEmpty, @NotBlank: These annotations are used to specify constraints on fields or method parameters, such as not allowing null, empty, or whitespace values.

3️⃣@Min, @Max, @Size: They define constraints on numeric values or the size of collections or strings.

4️⃣@Pattern: It validates the annotated element against a regular expression pattern.

## Spring Task Scheduling Annotations:
1️⃣ @EnableScheduling: This annotation enables Spring's task scheduling capabilities.

2️⃣@Scheduled: It is used to define a method as a scheduled task. You can specify the fixed rate, initial delay, or cron expression for executing the task.
## Spring Messaging Annotations:
1️⃣ @EnableWebSocket: This annotation enables WebSocket support in Spring applications.

2️⃣ @MessageMapping: It maps a specific WebSocket message to a method in a controller.

3️⃣ @SubscribeMapping: This annotation maps a WebSocket subscription message to a method in a controller.

## Spring Testing Annotations:
1️⃣ @RunWith: This annotation is used to specify the test runner class for running unit tests.

2️⃣ @SpringBootTest: It can be used to load and configure the complete Spring Boot application context for integration testing.

3️⃣ @MockBean: This annotation creates a mock implementation of a bean for testing purposes.

## Spring Integration Annotations:
1️⃣ @IntegrationComponentScan: This annotation enables component scanning for Spring Integration components.

2️⃣ @ServiceActivator: It is used to define a method as a service activator within a Spring Integration flow.

3️⃣@Transformer: This annotation marks a method as a transformer that converts input messages to output messages.

## Spring Cloud Annotations:
1️⃣ @EnableDiscoveryClient: This annotation enables service discovery capabilities for Spring Cloud applications.

2️⃣ @EnableFeignClients: It allows the generation of REST clients for performing declarative HTTP requests in a Spring Cloud application.

3️⃣ @EnableConfigServer: This annotation enables the Spring Cloud Config Server for externalized configuration management.

## There you have it! 🌟 These Spring Boot annotations are the building blocks of powerful and efficient applications. Mastering them will help you become a Spring Boot guru! Happy coding!