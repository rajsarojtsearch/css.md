1. Q: What is the Spring Framework?
   A: Spring is an open-source framework for building Java applications, providing features like dependency injection, aspect-oriented programming, and integration with various technologies.

2. Q: What are the core modules of the Spring Framework?
   A: Core modules include Spring Core, Spring Beans, Spring Context, Spring AOP, Spring JDBC, Spring ORM, Spring MVC, and Spring Security.

3. Q: What is Dependency Injection (DI) in Spring?
   A: DI is a design pattern where Spring injects dependencies into objects, reducing tight coupling and improving testability.

4. Q: Explain the difference between Constructor Injection and Setter Injection.
   A: Constructor Injection provides dependencies through a class constructor, while Setter Injection uses setter methods.

5. Q: What is the ApplicationContext in Spring?
   A: ApplicationContext is an advanced version of BeanFactory, providing additional features like event propagation and internationalization.

6. Q: What is the difference between BeanFactory and ApplicationContext?
   A: BeanFactory is a simple container, whereas ApplicationContext offers enterprise-specific features like event handling and declarative mechanisms.

7. Q: What are Spring Beans?
   A: Spring Beans are Java objects that Spring manages within its container.

8. Q: How do you define a Spring Bean?
   A: Beans can be defined using XML configuration, Java-based configuration, or annotations like @Component, @Service, and @Repository.

9. Q: What is Spring Boot?
   A: Spring Boot is a framework that simplifies Spring application development by providing pre-configured setups and embedded servers.

10. Q: How does Spring Boot simplify configuration?
    A: Spring Boot uses auto-configuration and opinionated defaults to reduce manual setup.

11. Q: What is Spring MVC?
    A: Spring MVC is a web framework based on the Model-View-Controller (MVC) pattern for building web applications.

12. Q: What are the key components of Spring MVC?
    A: DispatcherServlet, Controller, ViewResolver, Model, and View.

13. Q: What is @RestController in Spring Boot?
    A: @RestController is an annotation that combines @Controller and @ResponseBody, simplifying REST API development.

14. Q: What is Spring AOP?
    A: Aspect-Oriented Programming (AOP) helps in separating cross-cutting concerns like logging, security, and transaction management.

15. Q: What are different types of advice in Spring AOP?
    A: Before, After, Around, After Returning, and After Throwing advice.

16. Q: How does Spring handle transactions?
    A: Spring manages transactions using @Transactional annotation and PlatformTransactionManager.

17. Q: What is Spring Security?
    A: Spring Security is a framework for securing Java applications through authentication and authorization mechanisms.

18. Q: How does Spring Security handle authentication?
    A: It supports multiple authentication methods, such as form-based login, OAuth2, JWT, and LDAP.

19. Q: What is Spring Data JPA?
    A: Spring Data JPA simplifies data access by providing an abstraction over JPA implementations like Hibernate.

20. Q: What is the difference between CrudRepository and JpaRepository?
    A: CrudRepository provides basic CRUD operations, while JpaRepository extends it with additional JPA features.

21. Q: How do you enable caching in Spring?
    A: By using @EnableCaching and @Cacheable annotations.

22. Q: What is the difference between @Component, @Service, and @Repository?
    A: @Component is a general stereotype annotation, while @Service and @Repository are specialized for service and repository layers.

23. Q: What is Spring Cloud?
    A: Spring Cloud provides tools for building distributed systems and microservices.

24. Q: How do you handle exceptions in Spring MVC?
    A: By using @ExceptionHandler, @ControllerAdvice, or ResponseEntityExceptionHandler.

25. Q: What is the role of DispatcherServlet in Spring MVC?
    A: It acts as a front controller, handling requests and dispatching them to appropriate controllers.

26. Q: How do you configure CORS in Spring Boot?
    A: Using @CrossOrigin annotation or WebMvcConfigurer.

27. Q: What is Spring Actuator?
    A: A set of production-ready features in Spring Boot for monitoring and managing applications.

28. Q: What are Profiles in Spring Boot?
    A: Profiles allow defining different configurations for different environments (e.g., dev, test, prod).

29. Q: What is @Qualifier in Spring?
    A: It helps resolve conflicts when multiple beans of the same type exist.

30. Q: What is a Singleton Bean in Spring?
    A: A bean instance that is created once per Spring container.

31. Q: What is the difference between @Autowired and @Inject?
    A: @Autowired is Spring-specific, while @Inject is from JSR-330.

32. Q: How do you schedule tasks in Spring?
    A: Using @Scheduled annotation.

33. Q: What is a Proxy in Spring AOP?
    A: A Proxy intercepts method calls to apply cross-cutting concerns.

34. Q: How do you externalize configuration in Spring Boot?
    A: Using application.properties or application.yml files.

35. Q: What is Feign Client in Spring Cloud?
    A: Feign simplifies REST API calls by providing declarative REST clients.

36. Q: How does Spring Boot handle embedded servers?
    A: It includes embedded servers like Tomcat, Jetty, and Undertow.

37. Q: What is Circuit Breaker in Spring Cloud?
    A: It prevents cascading failures in microservices using Resilience4j or Hystrix.

38. Q: What is WebFlux in Spring?
    A: WebFlux is a reactive programming framework for non-blocking web applications.

39. Q: How does Spring Boot support internationalization (i18n)?
    A: By using ResourceBundleMessageSource.

40. Q: How do you implement logging in Spring Boot?
    A: Using SLF4J with Logback or Log4j.

41. Q: What is Lombok in Spring Boot?
    A: Lombok is a library that reduces boilerplate code using annotations like @Getter and @Setter.

42. Q: What is @Scope annotation in Spring?
    A: It defines the scope of a Spring Bean (e.g., singleton, prototype, request, session).

43. Q: What is Spring Batch?
    A: Spring Batch is a framework for batch processing large datasets.

44. Q: What is a RestTemplate?
    A: RestTemplate is used to make HTTP requests in Spring.

45. Q: What is WebClient in Spring WebFlux?
    A: WebClient is a reactive alternative to RestTemplate.

46. Q: What is a Spring Boot Starter?
    A: A starter is a pre-configured dependency set that simplifies project setup.

47. Q: What is Flyway in Spring Boot?
    A: Flyway is a database migration tool.

48. Q: How do you implement OAuth2 in Spring Boot?
    A: Using Spring Security OAuth2 Client or Resource Server.

49. Q: What is Spring Integration?
    A: A framework for enterprise integration patterns.

50. Q: What is the difference between Spring Boot and Spring Framework?
    A: Spring Boot simplifies Spring configuration, while Spring Framework provides core functionalities.
