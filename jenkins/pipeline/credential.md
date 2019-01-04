# Note: Not tested

# Credential in DSL plugin
https://jenkinsci.github.io/job-dsl-plugin/#plugin/credentials-binding

# withCredential 
https://support.cloudbees.com/hc/en-us/articles/204897020-Fetch-a-userid-and-password-from-a-Credential-object-in-a-Pipeline-job-

# credential for httprequest plugin
```
pipeline {
    agent any
    parameters {
        credentials credentialType: 'com.cloudbees.plugins.credentials.impl.UsernamePasswordCredentialsImpl', defaultValue: '', description: '', name: 'CredentialsForBackend', required: true
    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.CredentialsForBackend}"                
                httpRequest authentication: "${params.CredentialsForBackend}", consoleLogResponseBody: true, ignoreSslErrors: true, responseHandle: 'NONE', url: 'https://example.com/serveice/aabc'              
            }
        }
    }
}
```

# References
https://jenkins.io/doc/pipeline/steps/credentials-binding/
