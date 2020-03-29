# Artifactory OSS Memo


## Settings @ Artifactory

1. Security Configuration
    1. Allow anonymous access
1. Repositories > Remote
    1. central
        1. https://repo1.maven.org/maven2/
1. Repositories > Virtual
    1. public


## Local env

- http://localhost:8081/artifactory/
- http://localhost:8082/ui/

## Sample maven

### Start docker containers

    docker-compose build

    docker-compose up -d


### Download

    docker exec -it maven-download bash

    cd /root/maven/

    mvn -U dependency:resolve


### Upload

    docker exec -it gradle-upload bash

    cd /root/gradle




## References

- [How do I login to Artifactory for the first time? What are the default admin username and password?](https://www.jfrog.com/confluence/display/RT12/FAQs#FAQs-HowdoIlogintoArtifactoryforthefirsttime?Whatarethedefaultadminusernameandpassword?)
- [Artifactory OSS](https://www.jfrog.com/confluence/display/RTF5X/Installing+with+Docker)
