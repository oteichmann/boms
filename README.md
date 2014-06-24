WildFly JBoss BOMs
==================

The WildFly JBoss BOM's project provides Maven BOM files enhancing Java EE 7 with deployment and test tooling. These files manage the version of the dependencies you use in your project, ensuring you always get a compatible stack.

Usage
-----

To use the BOM, import into your dependency management. For example, if you wanted "Java EE with Tools recommended by WildFly", use:

    <dependencyManagement>    
        <dependencies>
            <dependency>
                <groupId>org.wildfly.bom</groupId>
                <artifactId>jboss-javaee-7.0-with-tools</artifactId>
                <version>8.1.0.Final</version>
                <scope>import</scope>
            </dependency>
        </dependencies>
    </dependencyManagement> 
	
Unfortunately, Maven doesn't allow you to specify plugin versions this way. The readme for each BOM calls out any plugin versions you should use. For example, to use the plugins associated with "Java EE with Tools recommended by WildFly":

    <pluginManagement>
        <plugins>
            <!-- The Maven Surefire plugin tests your application. Here we ensure we are using a version compatible with Arquillian -->
            <plugin>
                <artifactId>maven-surefire-plugin</artifactId>
                <version>2.17</version>
            </plugin>
            <!-- The WildFly Maven Plugin deploys your war to a local WildFly container -->
            <!-- To use, set the JBOSS_HOME environment variable and run:
                 mvn package wildfly:deploy -->
            <plugin>
                <groupId>org.wildfly.plugins</groupId>
                <artifactId>wildfly-maven-plugin</artifactId>
                <version>1.0.2.Final</version>
            </plugin>
        </plugins>
    </pluginManagement>

You'll need to take a look at the POM source in order to find the latest versions of plugins recommended.

