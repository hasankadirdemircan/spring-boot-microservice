# spring-boot-microservice
Thanks in28minutes for microservice udemy education,
<a href="https://www.udemy.com/course/microservices-with-spring-boot-and-spring-cloud/">Udemy Url</a>
spring-boot-microservice

<table>
	<td><a href="#"><img src="https://user-images.githubusercontent.com/34090058/67662717-00b71880-f975-11e9-8067-ca3c2062680a.png" width="200"></a></td>
	<td><a href="#"><img src="https://user-images.githubusercontent.com/34090058/69222719-14782800-0b8b-11ea-8a3c-048afb483682.png" width="200"></a></td>
<td><a href="#"><img src="https://user-images.githubusercontent.com/34090058/69222742-235eda80-0b8b-11ea-9591-c27748d1c79e.png" width="200"></a></td>
     <td><a href="#"><img src="https://user-images.githubusercontent.com/34090058/69222759-29ed5200-0b8b-11ea-874f-cf855c7c8469.png" width="200"></a></td>
    <td><a href="#"><img src="https://user-images.githubusercontent.com/34090058/69222770-31146000-0b8b-11ea-96c6-7a2012ff9fba.png" width="200"></a></td>
</table>

<p align="center">
  <a href="#">
    <img alt="Techs" title="Techs" src="" width="700">
  </a>
</p>


## Ports

|     Application       |     Port          |
| ------------- | ------------- |
| Limits Service | 8080, 8081, ... |
| Spring Cloud Config Server | 8888 |
|  |  |
| Currency Exchange Service | 8000, 8001, 8002, ..  |
| Currency Conversion Service | 8100, 8101, 8102, ... |
| Netflix Eureka Naming Server | 8761 |
| Netflix Zuul API Gateway Server | 8765 |
| Zipkin Distributed Tracing Server | 9411 |


## URLs

|     Application       |     URL          |
| ------------- | ------------- |
| Limits Service | http://localhost:8080/limits POST -> http://localhost:8080/actuator/refresh|
|Spring Cloud Config Server| http://localhost:8888/limits-service/default http://localhost:8888/limits-service/dev |
|  Currency Converter Service - Direct Call| http://localhost:8100/currency-converter/from/USD/to/INR/quantity/10|
|  Currency Converter Service - Feign| http://localhost:8100/currency-converter-feign/from/EUR/to/INR/quantity/10000|
| Currency Exchange Service | http://localhost:8000/currency-exchange/from/EUR/to/INR http://localhost:8001/currency-exchange/from/USD/to/INR|
| Eureka | http://localhost:8761/|
| Zuul - Currency Exchange & Exchange Services | http://localhost:8765/currency-exchange-service/currency-exchange/from/EUR/to/INR http://localhost:8765/currency-conversion-service/currency-converter-feign/from/USD/to/INR/quantity/10|
| Zipkin | http://localhost:9411/zipkin/ |
| Spring Cloud Bus Refresh | http://localhost:8080/bus/refresh |
