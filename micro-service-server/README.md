# micro-service-server

# startup dependencies
mysql、rabbitmq

# start application with the specified profile
add another application-dev.properties file to resources directory, and start application with the following command, mvn spring-boot:run -Dserver.port=9001 -Dspring.profiles.active=dev -Darchaius.configurationSource.additionalUrls=classpath:///application.properties

# monitor application
download turbine-web and hystrix-dashboard war files, modify the configurations refering to turbine.config.properties under resources directory, and start them with web servers