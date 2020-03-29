# Artifactory OSS Memo


## Settings @ Artifactory

1. Security Configuration
    1. Allow anonymous access
1. Repository > Repositories > Remote
    1. central
        1. https://repo1.maven.org/maven2/
        1.

## Local env

- http://localhost:8081/artifactory/
- http://localhost:8082/ui/

## Sample maven

### Download

    docker exec -it maven bash

    cp /root/maven/conf/settings.xml /usr/share/maven/conf/

    cd /root/maven/download/

    mvn -U dependency:resolve


## References

- [How do I login to Artifactory for the first time? What are the default admin username and password?](https://www.jfrog.com/confluence/display/RT12/FAQs#FAQs-HowdoIlogintoArtifactoryforthefirsttime?Whatarethedefaultadminusernameandpassword?)
- [Artifactory OSS](https://www.jfrog.com/confluence/display/RTF5X/Installing+with+Docker)
