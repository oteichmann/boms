WildFly JBoss Java EE 7 with Hibernate 3
================================

This BOM builds on the Java EE full profile BOM, adding Hibernate Community projects including Hibernate 3 ORM, Hibernate
Entity Manager (JPA 1.0) and Hibernate Validator.

Usage
-----

To use the BOM, import into your dependency management:

    <dependencyManagement>
        <dependencies>
	    <dependency>
	       <groupId>org.wildfly.bom</groupId>
               <artifactId>jboss-javaee-7.0-with-hibernate3</artifactId>
               <version>8.1.0.Final</version>
               <type>pom</type>
               <scope>import</scope>
            </dependency>
        </dependencies>
    </dependencyManagement> 

