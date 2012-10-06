Maven-repository
================

This is public maven repository for the [uri](https://github.com/justahero/uri) project.
Modify the `pom.xml` of your project in order to use the library of this repository.

First the location of the repository must be given.

````xml
<repositories>
    <repository>
        <id>URI snapshots</id>
        <url>https://raw.github.com/justahero/maven-repository/master/snapshots</url>
        <layout>default</layout>
    </repository>
</repositories>
````

Then the dependency must be specified.

````xml
<dependency>
    <groupId>com.uri</groupId>
    <artifactId>URI</artifactId>
    <version>0.2.1</version>
</dependency>
````

Once `mvn package` or `mvn install` is run for your project the dependent jar file is downloaded
and made available (put into the local `~/.m2/repository` folder).
In the example above the jar file `URI-0.2.1.jar` would be downloaded.
