# springboot-autoConfigure-redis
通过该篇教程-来学习springboot的自动配置原理 并写一个简单的spring-boot-redis-starter

##项目所使用技术

* [springboot](https://spring.io/projects/spring-boot)
* [redis官网](https://redis.io/)

##springboot自动配置的原理
* 启动类注解`@SpringBootApplication`该注解中包含了`@SpringBootConfiguration`,`@EnableAutoConfiguration`,`@ComponentScan`

* 注意到`@EnableAutoConfiguration`是一个派生注解,该注解中包含了`@AutoConfigurationPackage`, `@Import(AutoConfigurationImportSelector.class)`

* 让我们来看下`@Import`注解
