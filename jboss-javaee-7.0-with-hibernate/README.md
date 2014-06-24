WildFly JBoss Java EE 7 with Hibernate
==============================

This BOM builds on the Java EE full profile BOM, adding Hibernate Community projects including Hibernate ORM, Hibernate Search and Hibernate Validator.

It also provides tool projects such as Hibernate JPA Model Gen and Hibernate Validator Annotation Processor.

Usage
-----

To use the BOM, import into your dependency management:

    <dependencyManagement>
        <dependencies>
	    <dependency>
	       <groupId>org.wildfly.bom</groupId>
               <artifactId>jboss-javaee-7.0-with-hibernate</artifactId>
               <version>8.1.0.Final</version>
               <type>pom</type>
               <scope>import</scope>
            </dependency>
        </dependencies>
    </dependencyManagement> 

