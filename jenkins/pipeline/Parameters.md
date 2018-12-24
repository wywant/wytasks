# Parameters syntax
https://jenkins.io/doc/book/pipeline/syntax/#parameters

# Parameters Generator
http://localhost:8080/directive-generator/

# read credentials
AN_ACCESS_KEY = credentials('my-prefined-secret-text')  
https://jenkins.io/doc/book/pipeline/syntax/#environment

# References
https://medium.com/@Lenkovits/jenkins-pipelines-and-their-dirty-secrets-1-9e535cd603f4  


# Inheriting job variables from previous jobs
```
b = build( "job1", param1: "foo", param2: "bar" ) 
build( "job2", param1: b.build.number )
```

# Pipeline asking for input during build

# environment 
credentials add two variables _USR and _PSW 
```
environment {
      /*
       * Uses a Jenkins credential called "FOOCredentials" and creates environment variables:
       * "$FOO" will contain string "USR:PSW"
       * "$FOO_USR" will contain string for Username
       * "$FOO_PSW" will contain string for Password
       */
      FOO = credentials("FOOcredentials")
    }
    
    ...
    sh 'echo $FOO_PSW > foo_psw.txt'
    sh 'echo $FOO_USR > foo_usr.txt'
 ```
 
https://github.com/jenkinsci/pipeline-examples/blob/master/declarative-examples/simple-examples/credentialsMixedEnvironment.groovy
