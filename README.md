# Cereebro issue #97

Start the app and pass the Eureka Server credentials as arguments or environment variables :

 * `eureka.security.user.name`
 * `eureka.security.user.password`

Remove these variables in `application.yaml` if your Eureka Server is not using Spring Security.

To test with the sample: you can run :

`curl -i --url "http://localhost:8080/cereebro-sample-netflix-app1/hello"`
(you should receive _hello_ in the response)

It targets the service deployed here -> `https://cereebro-netflix-app1.herokuapp.com/hello`

You can hit the Cereebro Snitch endpoint to display downstream services : 

`curl -i --url "http://localhost:8080/cereebro/snitch"`
