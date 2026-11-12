# Java-CI

Minimal Java CI/CD setup using **Maven** for build/test and **Jenkins** for pipeline orchestration.

## Local validation

```bash
mvn clean verify
```

## Jenkins pipeline

The `Jenkinsfile` defines a declarative pipeline that:
- checks out the repository
- runs `mvn -B clean verify`
- publishes JUnit test reports
- archives generated JAR artifacts
