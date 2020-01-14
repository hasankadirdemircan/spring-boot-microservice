# spring-boot-microservice
Thanks in28minutes for microservice udemy education,
<a href="https://www.udemy.com/course/microservices-with-spring-boot-and-spring-cloud/">Udemy Url</a>
spring-boot-microservice

<td><a href="https://user-images.githubusercontent.com/34090058/67662717-00b71880-f975-11e9-8067-ca3c2062680a.png"><img src="https://user-images.githubusercontent.com/34090058/67662717-00b71880-f975-11e9-8067-ca3c2062680a.png" width=400"></a></td>
	<td><a href="https://user-images.githubusercontent.com/34090058/69222719-14782800-0b8b-11ea-8a3c-048afb483682.png"><img src="https://user-images.githubusercontent.com/34090058/69222719-14782800-0b8b-11ea-8a3c-048afb483682.png" width="400"></a></td>
<td><a href="https://user-images.githubusercontent.com/34090058/69222742-235eda80-0b8b-11ea-9591-c27748d1c79e.png"><img src="https://user-images.githubusercontent.com/34090058/69222742-235eda80-0b8b-11ea-9591-c27748d1c79e.png" width="400"></a></td>
     <td><a href="https://user-images.githubusercontent.com/34090058/69222759-29ed5200-0b8b-11ea-874f-cf855c7c8469.png"><img src="https://user-images.githubusercontent.com/34090058/69222759-29ed5200-0b8b-11ea-874f-cf855c7c8469.png" width="400"></a></td>
    <td><a href="https://user-images.githubusercontent.com/34090058/69222770-31146000-0b8b-11ea-96c6-7a2012ff9fba.png"><img src="https://user-images.githubusercontent.com/34090058/69222770-31146000-0b8b-11ea-96c6-7a2012ff9fba.png" width="400"></a></td>
	
## Mircoservice Screenshot

#### limits-service
</p>
<p>
  <a href="#">
    <img alt="Techs" title="Techs" src="https://user-images.githubusercontent.com/34090058/72368098-72019e80-370e-11ea-8b0a-09c86fff406a.png"width="300">
  </a>
</p>

</p>
<p>
  <a href="#">
    <img alt="Techs" title="Techs" src="https://user-images.githubusercontent.com/34090058/72368131-7fb72400-370e-11ea-9176-2ca8b8815e35.png"width="300">
  </a>
</p>

#### currency-exchange-service
</p>
<p>
  <a href="#">
    <img alt="Techs" title="Techs" src="https://user-images.githubusercontent.com/34090058/72368149-8776c880-370e-11ea-8a34-c6baeca592dd.png"width="300">
  </a>
</p>

#### api-gateway-server
</p>
<p>
  <a href="#">
    <img alt="Techs" title="Techs" src="https://user-images.githubusercontent.com/34090058/72368236-b725d080-370e-11ea-816c-824985069893.png"width="300">
  </a>
</p>

#### eureka-naming-server
</p>
<p>
  <a href="#">
    <img alt="Techs" title="Techs" src="https://user-images.githubusercontent.com/34090058/72368430-213e7580-370f-11ea-9fa6-a3d9e7f9dd0c.png"width="300">
  </a>
</p>

#### zipkin
</p>
<p>
  <a href="#">
    <img alt="Techs" title="Techs" src="https://user-images.githubusercontent.com/34090058/72368266-c7d64680-370e-11ea-9c1c-57e7814a6b79.png"width="300">
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
