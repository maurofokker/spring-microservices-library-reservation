# Spring microservice library reservation

* This service is part of the simple library microservices project and includes
  * [library configuration server](https://github.com/maurofokker/spring-microservices-library-config)
  * [library catalog](https://github.com/maurofokker/spring-microservices-library-catalog)
  * [library ui](https://github.com/maurofokker/spring-microservices-library-ui)
  * [library discovery & registry](https://github.com/maurofokker/spring-microservices-library-registry)
  * [library edge service](https://github.com/maurofokker/spring-microservices-library-edge)
* Microservices reference can be found [here](https://github.com/maurofokker/microservices-demo)
* To test load balancing run two instances of reservation service
  * Comment or delete `server.port=5000` in `application.properties` file
  * In run configurations use: `-Dserver.port=5006` for one instance and `-Dserver.port=5007` fot the second instance
* `Zuul Edge Service` perform a Load Balancing with `Ribbon` by default without additional configuration 