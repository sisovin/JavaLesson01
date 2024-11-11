# How to install jshell

## With PowerShell

in the Microsoft.PowerShell_profile.ps1 writes this line in:
$Env:Path = "C:\Program Files\Microsoft\jdk-17.0.11.9-hotspot\bin;" + $Env:Path

## With Zsh

in the .zshrc, we have to write the corrected line for our .zshrc file:
export PATH="/C/Program Files/Microsoft/jdk-17.0.11.9-hotspot:$PATH"

## With CMD prompt

to test the jshell after add the env: JAVA_HOME=C:\Program Files\Microsoft\jdk-17.0.11.9-hotspot\
echo %JAVA_HOME%

:\Users\DELL>jshell
| Welcome to JShell -- Version 17.0.3.1
| For an introduction type: /help intro

jshell> System.out.println("Hello World")
Hello World

jshell> System.out.println("Navin Reddy, Telusko")
Navin Reddy, Telusko

jshell> 2+4
$3 ==> 6

jshell> 9-6
$4 ==> 3

jshell>

Please generate Command line in Java language.

```Java
public class CommandLineExample {
    public static void main(String[] args) {
        // Check if at least one argument is provided
        if (args.length > 0) {
            System.out.println("Arguments provided:");
            for (String arg : args) {
                System.out.println(arg);
            }
        } else {
            System.out.println("No arguments provided.");
        }
    }
}
```

# Lesson 01: Introduction

## What is Java?

Java is a high-level, class-based, object-oriented programming language that is designed to have as few implementation dependencies as possible. It is a general-purpose programming language intended to let application developers write once, run anywhere (WORA), meaning that compiled Java code can run on all platforms that support Java without the need for recompilation. Java applications are typically compiled to bytecode that can run on any Java virtual machine (JVM) regardless of the underlying computer architecture.

1. **When was Java happened?**: Java was created in 1995 by James Gosling and his team at Sun Microsystems. It was initially released as part of the Java Development Kit (JDK) 1.0.
2. **Who is the creator?**: The creator of Java is James Gosling. He and his team at Sun Microsystems developed Java, and it was first released in 1995.
3. **Which company has belong of Java?**: Java was originally developed by Sun Microsystems. In 2010, Oracle Corporation acquired Sun Microsystems, and since then, Oracle has been responsible for the development and maintenance of Java.
4. **What types of Java are there?**: There are several editions of Java, each serving different purposes:

   1. **Java Standard Edition (Java SE)**: This is the core Java platform, which provides the basic libraries and APIs for building desktop and server applications.

   2. **Java Enterprise Edition (Java EE)**: Now known as Jakarta EE, this edition builds on Java SE and provides additional libraries and APIs for building large-scale, distributed, and multi-tiered enterprise applications.

   3. **Java Micro Edition (Java ME)**: This edition is designed for resource-constrained devices such as embedded systems, mobile phones, and other small devices.

   4. **JavaFX**: A platform for creating rich internet applications using a lightweight user interface API.

These editions cater to different types of applications and development environments.

## What are some popular Java frameworks and libraries?

Some popular Java frameworks and libraries include:

1. **Spring Framework**: A comprehensive framework for enterprise Java development, providing support for dependency injection, aspect-oriented programming, and more.

2. **Hibernate**: An object-relational mapping (ORM) library for Java, simplifying database interactions by mapping Java classes to database tables.

3. **Apache Struts**: A framework for building web applications using the Model-View-Controller (MVC) architecture.

4. **JavaServer Faces (JSF)**: A Java specification for building component-based user interfaces for web applications.

5. **Apache Maven**: A build automation tool used primarily for Java projects, managing project dependencies and build lifecycle.

6. **JUnit**: A widely used testing framework for Java, supporting the creation and execution of unit tests.

7. **Log4j**: A logging library for Java, providing a flexible and efficient way to log messages from Java applications.

8. **Gson**: A library for converting Java objects to JSON and vice versa.

9. **Apache Commons**: A collection of reusable Java components, providing utilities for various tasks such as file manipulation, collections, and more.

10. **Jackson**: A library for processing JSON data, including parsing, generating, and data binding.

These frameworks and libraries help developers build robust, scalable, and maintainable Java applications.

## What are some popular Integrated Development Environments (IDEs) for Java development?

Some popular Integrated Development Environments (IDEs) for Java development include:

1. **IntelliJ IDEA**: A powerful and feature-rich IDE developed by JetBrains, known for its intelligent code completion, refactoring tools, and deep integration with various frameworks and tools.

2. **Eclipse**: An open-source IDE with a large ecosystem of plugins, providing extensive support for Java development and other programming languages.

3. **NetBeans**: An open-source IDE maintained by the Apache Software Foundation, offering robust support for Java development, including tools for debugging, profiling, and code analysis.

4. **Visual Studio Code**: A lightweight, open-source code editor developed by Microsoft, which can be extended with various plugins to support Java development.

These IDEs provide a range of features to enhance productivity, such as code completion, debugging, version control integration, and more.

## What are some popular Java build tools?

Some popular Java build tools include:

1. **Apache Maven**: A build automation tool used primarily for Java projects, managing project dependencies, build lifecycle, and project configuration through a standardized XML file called `pom.xml`.

2. **Gradle**: A flexible and powerful build automation tool that uses a Groovy-based DSL (Domain Specific Language) for configuration. It supports incremental builds and is known for its performance and scalability.

3. **Ant**: A Java-based build tool from Apache that uses XML to describe the build process and its dependencies. It is highly customizable and can be extended with custom tasks.

These build tools help automate the process of compiling, packaging, testing, and deploying Java applications.

## What are some popular Java web frameworks?

Some popular Java web frameworks include:

1. **Spring MVC**: Part of the Spring Framework, it provides a comprehensive infrastructure for building web applications, including support for RESTful services, form handling, and more.

2. **JavaServer Faces (JSF)**: A Java specification for building component-based user interfaces for web applications, simplifying the development of server-side user interfaces.

3. **Struts**: An open-source framework for building web applications using the Model-View-Controller (MVC) architecture, providing a robust infrastructure for developing scalable web applications.

4. **Play Framework**: A reactive web application framework that follows the MVC pattern, designed for high performance and scalability, and supports both Java and Scala.

5. **Vaadin**: A framework for building modern web applications with a rich user interface, allowing developers to write UI components in Java.

These frameworks help developers create robust, scalable, and maintainable web applications in Java.

## What are some popular Java testing frameworks?

Some popular Java testing frameworks include:

1. **JUnit**: A widely used testing framework for Java, supporting the creation and execution of unit tests. It provides annotations to identify test methods and assertions to test expected outcomes.

2. **TestNG**: Inspired by JUnit, TestNG is a testing framework designed to cover a wider range of test categories, including unit, functional, end-to-end, and integration tests. It offers more flexible test configuration and powerful features like data-driven testing.

3. **Mockito**: A mocking framework for Java that allows developers to create mock objects for unit testing, enabling the isolation of the code being tested from its dependencies.

4. **AssertJ**: A fluent assertion library for Java, providing a rich set of assertions and a readable, fluent API for writing assertions in tests.

5. **Cucumber**: A testing framework that supports Behavior-Driven Development (BDD), allowing developers to write tests in a natural language that can be understood by non-technical stakeholders.

6. **Arquillian**: A testing platform for Java that simplifies integration testing by managing the lifecycle of the container and deployment of the test archive.

These frameworks help developers ensure the quality and reliability of their Java applications through various types of testing.

## What are some popular Java database access frameworks?

Some popular Java database access frameworks include:

1. **Hibernate**: An object-relational mapping (ORM) framework that simplifies database interactions by mapping Java classes to database tables, allowing developers to work with data in an object-oriented way.

2. **Java Persistence API (JPA)**: A specification for ORM in Java, providing a standard way to manage relational data in Java applications. Hibernate is one of the most popular implementations of JPA.

3. **MyBatis**: A persistence framework that provides support for custom SQL, stored procedures, and advanced mappings. It allows developers to write SQL queries directly and map them to Java objects.

4. **Spring Data JPA**: Part of the Spring Data project, it simplifies data access by providing a repository abstraction over JPA, reducing the amount of boilerplate code needed for database operations.

5. **JDBC (Java Database Connectivity)**: A standard Java API for connecting to relational databases, executing SQL queries, and retrieving results. It provides a low-level interface for database access.

These frameworks help developers interact with databases more efficiently and effectively, providing various levels of abstraction and convenience.

## What is JVM technology?

The Java Virtual Machine (JVM) is a crucial component of the Java platform. It is a virtual machine that enables a computer to run Java programs as well as programs written in other languages that are compiled to Java bytecode. Here are some key aspects of JVM technology:

1. **Bytecode Execution**: The JVM executes Java bytecode, which is the compiled form of Java source code. This allows Java programs to be platform-independent, as the same bytecode can run on any device with a compatible JVM.

2. **Memory Management**: The JVM handles memory allocation and garbage collection, which helps manage the lifecycle of objects and ensures efficient use of memory.

3. **Security**: The JVM provides a secure execution environment by enforcing access controls and preventing unauthorized code from performing harmful operations.

4. **Performance Optimization**: The JVM includes Just-In-Time (JIT) compilation, which translates bytecode into native machine code at runtime, improving the performance of Java applications.

5. **Platform Independence**: By abstracting the underlying hardware and operating system, the JVM allows Java applications to run on any platform that has a compatible JVM implementation.

Overall, the JVM is a powerful and flexible technology that underpins the portability, security, and performance of Java applications.

## The powerfull language to connect with Oracle Database, mySQL Database, SQLLite, and MSSQL Server, as well as the none-database JSON, MongoDB

Java is a powerful language for connecting with various databases and data storage systems, including relational databases like Oracle Database, MySQL, SQLite, and Microsoft SQL Server, as well as non-relational databases like JSON and MongoDB. Here are some ways Java can interact with these systems:

1. **Relational Databases**:

   - **JDBC (Java Database Connectivity)**: A standard API for connecting and executing queries on relational databases. JDBC drivers are available for Oracle, MySQL, SQLite, MSSQL Server, and many other databases.
   - **Hibernate**: An ORM framework that simplifies database interactions by mapping Java objects to database tables.
   - **Spring Data JPA**: Part of the Spring Data project, it provides a repository abstraction over JPA, making it easier to work with relational databases.

2. **Non-Relational Databases**:
   - **JSON**: Libraries like Gson and Jackson can be used to parse and generate JSON data.
   - **MongoDB**: The MongoDB Java Driver provides a way to connect and interact with MongoDB databases. Additionally, Spring Data MongoDB offers a higher-level abstraction for working with MongoDB.

Java's extensive ecosystem of libraries and frameworks makes it a versatile choice for interacting with a wide range of data storage systems.
