# Parameters syntax
https://jenkins.io/doc/book/pipeline/syntax/#parameters

# Parameters Generator
http://localhost:8080/directive-generator/



# References
https://medium.com/@Lenkovits/jenkins-pipelines-and-their-dirty-secrets-1-9e535cd603f4  


# Inheriting job variables from previous jobs
```
b = build( "job1", param1: "foo", param2: "bar" ) 
build( "job2", param1: b.build.number )
```

# Pipeline asking for input during build
