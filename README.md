# SpringBootSample-microservice-forexservice

# To start new instance on another port like 8001 to test Ribbon Load Balancing Eureka Naming Server, follow below steps

1. In eclipse, goto Run -> Run Configurations

2. Right-click the Forex Service running (assuming FS service is imported in eclipse and running on port 8000) and select duplicate

3. For the instance duplicated, in the configurations window, goto Arguments

4. Add -Dserver.port=8001 in VM arguments sub window and select Run

# Testing, check for ports in output to determine the load balancing concept

http://localhost:8000/currency-exchange/from/USD/to/INR

http://localhost:8100/currency-converter/from/EUR/to/INR/quantity/10000

http://localhost:8100/currency-converter-feign/from/EUR/to/INR/quantity/10000

http://localhost:8100/currency-converter-feign/from/EUR/to/INR/quantity/10000

# Reference

https://github.com/in28minutes/spring-boot-examples/tree/master/spring-boot-basic-microservice

http://www.springboottutorial.com/creating-microservices-with-spring-boot-part-1-getting-started

http://www.springboottutorial.com/creating-microservices-with-spring-boot-part-2-forex-microservice

http://www.springboottutorial.com/creating-microservices-with-spring-boot-part-3-currency-conversion-microservice

http://www.springboottutorial.com/microservices-with-spring-boot-part-4-ribbon-for-load-balancing

http://www.springboottutorial.com/microservices-with-spring-boot-part-5-eureka-naming-server
