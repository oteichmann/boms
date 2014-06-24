WildFly JBoss Java EE 7 with ALL
===============================

This BOM builds on the Java EE full profile BOM, adding all JBoss BOMs.
 
Usage
-----

To use the BOM, import into your dependency management:

    <dependencyManagement>
        <dependencies>
            <dependency>
               <groupId>org.wildfly.bom</groupId>
               <artifactId>jboss-javaee-7.0-with-all</artifactId>
               <version>8.1.0.Final</version>
               <type>pom</type>
               <scope>import</type>
            </dependency>
        </dependencies>
    </dependencyManagement>
