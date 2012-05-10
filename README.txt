This is a simple example showing how to configure AspectJ's Load-time Weaving with 
Spring 2.5's <context:load-time-weaver/> to gather statistics.

Note: This example must be run with Java 5 or higher since support for the 
-javaagent JVM argument was added in Java 5. Also, Maven and Eclipse are 
currently configured to look for the spring-agent.jar at 
c:/spring-framework-2.5/dist/weaving/spring-agent.jar so you will need to 
edit this to match where it is actually located. This can be changed at the bottom of the 
Maven pom.xml or in the Eclipse Run Dialog's argument tab.

This project can be built using Maven (http://maven.apache.org).  It can also be imported into 
the Eclipse IDE, but the Maven repository variable will need to be set and the Maven build 
will need to be run at least once if you don't already have all the jars the project needs 
downloaded to your local Maven repository.  The project is also setup to use the 
Spring IDE (http://springide.org).

	mvn -Declipse.workspace=<path-to-eclipse-workspace> eclipse:add-maven-repo