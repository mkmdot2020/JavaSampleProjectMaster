# simple-java-maven-app

This repository is for the
[Build a Java app with Maven](https://jenkins.io/doc/tutorials/build-a-java-app-with-maven/)
tutorial in the [Jenkins User Documentation](https://jenkins.io/doc/).

The repository contains a simple Java application which outputs the string
"Hello world!" and is accompanied by a couple of unit tests to check that the
main application works as expected. The results of these tests are saved to a
JUnit XML report.

The `jenkins` directory contains an example of the `Jenkinsfile` (i.e. Pipeline)
you'll be creating yourself during the tutorial and the `jenkins/scripts` subdirectory
contains a shell script with commands that are executed when Jenkins processes
the "Deliver" stage of your Pipeline.
# JavaSampleProjectMaster

A Java application built with Apache Maven. Its main class is
`com.mycompany.app.App`, located at
`src/main/java/com/mycompany/app/App.java`.

## Requirements

- A JDK compatible with the Java version configured in `pom.xml`
- Apache Maven

The `pom.xml` file defines the project's Maven coordinates, Java version,
dependencies, and build configuration.

## Build and test

Run the test suite from the project root:

```shell
mvn clean test
```

Package the project:

```shell
mvn package
```

Maven places compiled classes and package artifacts in `target/`.

## Run the application

Compile the project and launch its main class:

```shell
mvn compile
java -cp target/classes com.mycompany.app.App
```

## Project layout

```text
pom.xml
src/
  main/java/com/mycompany/app/App.java
  test/java/                 # Add test sources here
```

Add production code under `src/main/java`, tests under `src/test/java`, and
manage dependencies and build settings in `pom.xml`.
