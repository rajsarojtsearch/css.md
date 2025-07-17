1. Q: What is java?
   A: Java is a high-level, object-oriented programming language developed by Sun Microsystems (now owned by Oracle). It is platform-independent due to its JVM (Java Virtual Machine).

2. Q: What are the key features of Java?
   A: Java is platform-independent, object-oriented, secure, robust, multi-threaded, and supports automatic memory management (Garbage Collection).

3. Q: What is the difference between JDK, JRE, and JVM?
   A: JDK (Java Development Kit) contains JRE (Java Runtime Environment) and development tools. JRE provides libraries and JVM (Java Virtual Machine) to execute Java programs.

4. Q: What is the purpose of the ‘static’ keyword in Java?
   A: The ‘static’ keyword is used to create class-level members that can be accessed without creating an object of the class.

5. Q: What is the difference between ‘==’ and ‘equals()’ in Java?
   A: ‘==’ compares object references, whereas ‘equals()’ compares object content (if overridden in a class like String).

6. Q: What is the difference between method overloading and method overriding?
   A: Overloading occurs when multiple methods have the same name but different parameters. Overriding occurs when a subclass provides a specific implementation for a method in its superclass.

7. Q: What is a constructor in Java?
   A: A constructor is a special method that initializes an object. It has the same name as the class and does not return any value.

8. Q: What is the difference between an interface and an abstract class?
   A: An abstract class can have both abstract and concrete methods, while an interface only has abstract methods (until Java 8, where default methods were introduced).

9. Q: What is the significance of the ‘final’ keyword?
   A: ‘final’ can be used for variables (constants), methods (prevent overriding), and classes (prevent inheritance).

10. Q: What is exception handling in Java?
    A: Exception handling is a mechanism to handle runtime errors using try, catch, finally, throw, and throws keywords.

11. Q: What is the difference between checked and unchecked exceptions?
    A: Checked exceptions are checked at compile-time (e.g., IOException), whereas unchecked exceptions occur at runtime (e.g., NullPointerException).

12. Q: What is multi-threading in Java?
    A: Multi-threading allows concurrent execution of two or more threads to maximize CPU utilization.

13. Q: How do you create a thread in Java?
    A: By extending the Thread class or implementing the Runnable interface.

14. Q: What is synchronization in Java?
    A: Synchronization prevents multiple threads from accessing a critical section of code simultaneously, ensuring data consistency.

15. Q: What is the difference between HashMap and Hashtable?
    A: HashMap is not synchronized, while Hashtable is synchronized and thread-safe.

16. Q: What is a lambda expression in Java?
    A: A lambda expression provides a clear and concise way to represent an anonymous function.

17. Q: What is the difference between ArrayList and LinkedList?
    A: ArrayList is backed by a dynamic array and provides fast random access, while LinkedList is implemented using a doubly linked list and provides efficient insertion/deletion.

18. Q: What is garbage collection in Java?
    A: Garbage collection automatically removes unused objects from memory to free up space.

19. Q: What is the difference between stack and heap memory?
    A: Stack memory stores method calls and local variables, while heap memory stores objects dynamically allocated at runtime.

20. Q: What is a functional interface in Java?
    A: A functional interface has exactly one abstract method and can be used with lambda expressions.

21. Q: What is the purpose of the ‘transient’ keyword in Java?
    A: The ‘transient’ keyword prevents a variable from being serialized.

22. Q: What is reflection in Java?
    A: Reflection allows inspecting and manipulating classes, methods, and fields at runtime.

23. Q: What are design patterns in Java?
    A: Design patterns are reusable solutions to common software design problems, such as Singleton, Factory, and Observer patterns.

24. Q: What is the difference between deep copy and shallow copy?
    A: A deep copy creates a new independent object, while a shallow copy only copies references to the original object.

25. Q: What is JDBC?
    A: JDBC (Java Database Connectivity) is an API that allows Java applications to interact with databases.

26. Q: What is Spring Framework?
    A: Spring is a lightweight Java framework for building enterprise applications with features like dependency injection and AOP.

27. Q: What is Hibernate?
    A: Hibernate is an ORM (Object-Relational Mapping) framework that simplifies database interactions in Java.

28. Q: What is a RESTful API in Java?
    A: A RESTful API is an API that follows REST principles and uses HTTP methods (GET, POST, PUT, DELETE) for communication.

29. Q: What is dependency injection in Java?
    A: Dependency injection is a design pattern where dependencies are injected into a class instead of being created inside it.

30. Q: What is the difference between SOAP and REST?
    A: SOAP is a protocol that uses XML for message exchange, while REST is an architectural style that supports multiple formats like JSON.

31. Q: What is an annotation in Java?
    A: Annotations provide metadata about code and are used for configuration, documentation, and runtime processing.

32. Q: What is serialization in Java?
    A: Serialization converts an object into a byte stream for storage or transmission.

33. Q: What is the Java Memory Model (JMM)?
    A: The JMM defines how threads interact through memory and guarantees visibility and ordering of shared variables.

34. Q: What is a daemon thread in Java?
    A: A daemon thread runs in the background and terminates when all user threads finish execution.

35. Q: What is an Enum in Java?
    A: An Enum is a special data type used to define collections of constants.

36. Q: What is the difference between String, StringBuffer, and StringBuilder?
    A: String is immutable, while StringBuffer and StringBuilder are mutable. StringBuilder is faster than StringBuffer as it is not synchronized.

37. Q: What is a Proxy class in Java?
    A: A Proxy class allows creating dynamic implementations of interfaces at runtime.

38. Q: What is method reference in Java?
    A: A method reference is a shorthand notation of a lambda expression to refer to an existing method.

39. Q: What is the difference between Comparator and Comparable?
    A: Comparable is used for natural ordering, whereas Comparator allows custom sorting logic.

40. Q: What is the default scope of a bean in Spring?
    A: The default scope of a Spring bean is singleton.

41. Q: What is Autowiring in Spring?
    A: Autowiring automatically injects dependencies into beans using annotations like @Autowired.

42. Q: What is the difference between @Component, @Service, and @Repository?
    A: @Component is a generic annotation, @Service is for service layer, and @Repository is for DAO layer.

43. Q: What is Lazy Loading in Hibernate?
    A: Lazy loading delays the loading of objects until they are needed.

44. Q: What is a Microservice?
    A: A microservice is an independent, loosely coupled service that performs a specific function.

45. Q: What is the role of an API Gateway in Microservices?
    A: API Gateway manages API requests, authentication, and rate limiting.

46. Q: What is the difference between SOAP Web Services and REST Web Services?
    A: SOAP uses XML and strict standards, while REST is more flexible and supports multiple data formats.

47. Q: What is the purpose of the ‘volatile’ keyword?
    A: The ‘volatile’ keyword ensures that a variable's value is always read from main memory.

48. Q: What is the Observer Design Pattern?
    A: The Observer pattern allows multiple objects to listen for changes in a subject.

49. Q: What is the difference between Executors and Threads in Java?
    A: Executors manage thread pools, while threads represent individual tasks.

50. Q: How do you handle memory leaks in Java?
    A: Use proper resource management, avoid circular references, and utilize profiling tools.
