# springCloudLearn
一、什么是微服务？  
&nbsp;&nbsp;&nbsp;&nbsp;微服务是系统架构上的一种设计风格，它的主旨将原本独立的系统拆分成多个小型的服务，这些小型服务都在各自独立的进程中运行，服务之间都是通过基于Http的Restful API进行通信协作。  
二、微服务架构的特性  
&nbsp;&nbsp;1)服务组件化  
&nbsp;&nbsp;2)业务团队化  
&nbsp;&nbsp;3)服务产品化  
&nbsp;&nbsp;4)服务平衡化  
&nbsp;&nbsp;5)去中心化治理  
&nbsp;&nbsp;6)去中心化管理数据  
&nbsp;&nbsp;7)运维自动化  
&nbsp;&nbsp;8)容错设计  
&nbsp;&nbsp;9)演进式设计  
三、springcloud是基于springboot实现的微服务框架开发工具  
微服务架构中涉及内容如下：配置管理、服务治理、断路器、智能路由、微代理、控制总线、全局锁、决策竞选、分布式会话、集群状态管理。  
1、配置管理  
spring could config：配置管理工具，支持使用git存储配置内容，可以使用它实现应用配置的外部化存储，并支持客户端信息刷新、加密/解密配置内容。配置管理工具，支持使用git存储配置内容，可以使用它实现应用配置的外部化存储，并支持客户端信息刷新、加密/解密配置内容。  
Archaius：外部化配置组件  
2、服务治理  
Eureka：服务治理组件，包括服务注册中心、服务注册与发现机制的实现。
Spring cloud Consul：服务发现与配置管理工具。 
spring cloud zookeeper：基于Zookeeper的服务发现与配置管理组件。     
3、断路器  
Hystrix：容错管理组件，实现断路器模式，帮助服务依赖中出现的延迟和为故障提供强大的容错能力。  
4、智能路由  
Ribbon：客户端负载均衡的服务调用组件。  
Zuul：网关组件，提供智能路由、访问过滤等功能。  
5、微代理  
Feign：基于Ribbon和Hystrix的声明式服务调用组件。  
6、控制总线  
Spring cloud bus：事件、消息总线，用于传播集群中的状态变化或事件，以触发后续的处理，比如用来动态刷新配置等。  
spring cloud stream：通过Redis、Rabbit或者Kafka实现的消费微服务，可以通过简单的声明式模型来发送和接收消息。   
7、分布式跟踪  
Spring cloud Sleuth：Spring cloud应用的分布式跟踪实现，可以完美整合zipkin。    
8、集群状态管理  
spring cloud cluster:针对Zookeeper、Redis、Hazelcast、Consul的选举算法和通用状态模式的实现。  
9、安全  
spring cloud security：安全工具包，提供在Zuul代理中对Oauth2客户端请求的中继器。  
10、整合  
spring cloud aws：用于简化整合Amazon Web service的组件。  
spring cloud cloudFoundry：与Pivotal cloudfoundry的整合支持。  
四、springboot与springcloud的版本关系  
| Spring Cloud | Spring Boot |
| ------ | ------ |
| Finchley	| 兼容Spring Boot 2.0.x，不兼容Spring Boot 1.5.x |
| Dalston和Edgware | 兼容Spring Boot 1.5.x，不兼容Spring Boot 2.0.x |
| Camden | 兼容Spring Boot 1.4.x，也兼容Spring Boot 1.5.x |
| Brixton | 兼容Spring Boot 1.3.x，也兼容Spring Boot 1.4.x |
| Angel	| 兼容Spring Boot 1.2.x |

