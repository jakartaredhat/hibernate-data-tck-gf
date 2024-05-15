# Jakarta Data TCK Runner for Hibernate + WildFly

This project is a Jakarta Data TCK runner for Hibernate + WildFly. It is a simple project that demonstrates how to run
the Jakarta Data TCK tests against Hibernate on WildFly.

## Install the GlassFish server
Go to https://www.eclipse.org/downloads/download.php?file=/ee4j/glassfish/web-7.0.14.zip
and download the zip archive.

## Initialize the GlassFish server
There is a install-glassfish profile that will configure a local target/glassfish7 install with patched org.hibernate, jakarta.data.api  To use it, run:

```shell
mvn -Pstaging -Pinstall-glassfish clean process-sources
```

## Run the ValidationTests
Load the ee.jakarta.tck.data.web.validation.ValidationTests class in IntelliJ and run the tests.
