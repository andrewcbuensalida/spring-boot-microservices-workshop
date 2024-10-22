https://www.youtube.com/watch?v=e09P-CkCvvs

##
When running, was getting this error:
`Error: Could not find or load main class org.apache.maven.wrapper.MavenWrapperMain`

So went in each app's folder and ran this:
`mvn -N io.takari:maven:wrapper`
This created a .mvn folder


Now when doing Explorer > Maven > movie-info-service (for example) > Plugins > spring-boot > run, it errors:
`Caused by: org.springframework.beans.BeanInstantiationException: Failed to instantiate [org.springframework.cloud.context.properties.ConfigurationPropertiesBeans]: Factory method 'configurationPropertiesBeans' threw exception with message: org/springframework/boot/context/properties/ConfigurationBeanFactoryMetadata`

Upgraded spring-cloud.version to 2023 and has a warning:
`Dependency conflict in spring-cloud-starter-netflix-eureka-server: com.google.guava:guava:14.0.1 conflict with 33.0.0-jre`
##
