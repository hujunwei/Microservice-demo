# microservices-demo

![image](https://user-images.githubusercontent.com/6505469/169628610-386b8d2a-d08d-4954-89c0-947a4a6f02a7.png)


## 项目名称

microservices-demo

## 项目模块

### microservices-dependency

pom方式;项目总依赖包;通用的依赖版本;总体父项目

### microservices-commons

jar包方式;项目公共包;包含通用实体类,工具类,结果码等.

### microservices-eureka

项目注册中心;可做集群 ; 默认端口 8761;
应用名称(spring.application.name) : microservices-eureka
端口规划 : 7000 ; 集群规划 7000,7001,7002;

### microservices-order

订单服务接口 ; 可做集群 ; 默认端口 8000
应用名称(spring.application.name) : microservices-order
端口规划 : 8000 - 8199

### microservices-order-api

订单服务 ; 实际调用microservices-order ; 可做集群 ; 默认端口 8200
应用名称(spring.application.name) : microservices-order-api
端口规划 : 8200 - 8399

### microservices-goods

商品服务接口 ; 可做集群 ; 默认端口 8400
应用名称(spring.application.name) : microservices-goods
端口规划 : 8400 - 8599

### microservices-goods-api
商品服务 ; 实际调用microservices-goods; 可做集群 ; 默认端口 8600
应用名称(spring.application.name) : microservices-goods-api
端口规划 : 8600 - 8799
