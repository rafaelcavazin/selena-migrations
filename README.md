### Steps:

- must have java installed.
- brew install maven
- just run make

```
make
```
- adjust liquidbase properties
- adjust selena.changelog-master.xml
- add your changes

and then all you need is to run:

```
mvn liquibase:update -Denvironment=(development/uat/prod)
```
