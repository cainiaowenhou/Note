# 什么是 Spring 框架?
- 开源的轻量级 Java 开发框架，旨在提高开发人员的开发效率以及系统的可维护性
- 支持 IoC（Inversion of Control:控制反转） 和 AOP(Aspect-Oriented Programming:面向切面编程)
- 很方便地对数据库(JDBC、JPA)进行访问、可以很方便地集成第三方组件
# Spring,Spring MVC,Spring Boot 之间什么关系?
- Spring：Spring 是一个综合性的框架，用于构建企业级 Java 应用程序。它提供了许多模块和功能，包括依赖注入、面向切面编程、事务管理、数据访问、消息传递等。Spring 的目标是简化 Java 开发，提高代码的可维护性和可测试性。Spring 提供了核心容器、数据访问/集成、Web、AOP（面向切面编程）等多个模块。

- Spring MVC：Spring MVC 是 Spring 框架的一部分，用于构建基于模型-视图-控制器（MVC）设计模式的 Web 应用程序。它提供了一种结构化的方式来处理 HTTP 请求和响应，并将应用程序分为模型（Model）、视图（View）和控制器（Controller）。Spring MVC 可以帮助开发人员构建灵活且可扩展的 Web 应用程序，它通常与 Spring 框架一起使用。

- Spring Boot：Spring Boot 是 Spring 生态系统中的一个子项目，旨在简化 Spring 应用程序的创建和配置。它提供了一个约定优于配置的方式，使得开发者可以更容易地创建独立的、可运行的 Spring 应用程序。Spring Boot 包含了许多默认配置，因此你不必手动配置大量的参数和选项，可以更专注于编写业务逻辑。Spring Boot 还提供了嵌入式 Web 服务器（如Tomcat、Jetty等）的支持，使得创建自包含的 Web 应用程序变得非常容易。
#  Spring IoC 的了解?
-  是一种设计思想, 控制：指的是对象创建（实例化、管理）的权力,控制权交给外部环境（Spring 框架、IoC 容器）
-  作用：对象之间的耦合度或者说依赖程度降低
-  实现：工厂模式+反射机制
# 什么是 AOP？
- 面向切面编程
- AOP 的目的是将横切关注点（如日志记录、事务管理、权限控制）从核心业务逻辑中分离出来，通过动态代理等技术，实现代码的复用和解耦
- OOP 的目的是将业务逻辑按照对象的属性和行为进行封装，通过类、对象、继承、多态等概念，实现代码的模块化和层次化
- 提高代码的可维护性和可读性

# 什么是 Spring Bean？
- Bean 代指的就是那些被 IoC容器所管理的对象
- IoC容器帮助我们管理哪些对象，这个是通过配置元数据来定义的。配置元数据可以是 XML 文件、注解或者 Java 配置类。
# 将一个类声明为 Bean 的注解有哪些?
- @Component：通用的注解，可标注任意类为 Spring 组件。如果一个 Bean 不知道属于哪个层，可以使用@Component 注解标注。
- @Repository : 对应持久层即 Dao 层，主要用于数据库相关操作。
- @Service : 对应服务层，主要涉及一些复杂的逻辑，需要用到 Dao 层。
- @Controller : 对应 Spring MVC 控制层，主要用于接受用户请求并调用 Service 层返回数据给前端页面

