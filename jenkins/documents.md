http://www.ibm.com/developerworks/cn/java/j-lo-jenkins-plugin/index.html

https://wiki.jenkins-ci.org/display/JENKINS/Extend+Jenkins

https://github.wdf.sap.corp/ContinuousDelivery/jenkins-pipelines/blob/master/README.md

http://javadoc.jenkins.io/archive/jenkins-2.19/hudson/model/package-summary.html

http://stackoverflow.com/questions/12221799/how-to-customize-jenkins-build-name
https://dzone.com/refcardz/continuous-delivery-with-jenkins-workflow

https://github.com/jenkinsci/pipeline-examples/blob/master/docs/BEST_PRACTICES.md


http://javadoc.jenkins.io/archive/jenkins-2.19/hudson/model/package-summary.html

https://jenkins.io/doc/pipeline/steps/
https://github.com/jenkinsci/pipeline-plugin/blob/master/TUTORIAL.md

http://jenkins-ci.361315.n4.nabble.com/Pipeline-How-to-access-Jenkins-build-information-from-pipeline-td4835909.html

As for the error you are getting, it's the sandbox policies that block the execution for "security" reason. 
Either use case:
1- You use the direct pipeline script: You can disable it into the project pipeline config page by unchecking the Use Groovy Sandbox
2- You use scm to fetch the jenkinsfile: You need to go into the Manage Jenkins and then click on In-process Script Approval and approve the wanted function until the script pass for every script possible branches.

https://github.com/jenkinsci/pipeline-examples/blob/master/docs/BEST_PRACTICES.md


https://wiki.jenkins-ci.org/display/JENKINS/Script+Security+Plugin	



