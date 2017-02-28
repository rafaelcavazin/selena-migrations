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
- add a copy of your liquibase.properties with your passwords
- add a env.var like SELENA_MIGRATIONS_UAT and SELENA_MIGRATIONS_PROD
- point your env.var to your properties file.

and then all you need is to run:

```
mvn liquibase:update@acceptance
```

or

```
mvn liquibase:update@production
```
