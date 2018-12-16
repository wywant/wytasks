# Note
未经测试
# Read Jenkins Job common information
## env
### Global env variables
JENKINS_HOME JENKINS_URL
### Job env variables
JOB_NAME JOB_BASE_NAME  WORKSPACE

### Build env variables
BUILD_NUMBER BUILD_ID BUILD_DISPLAY_NAME  BUILD_TAG ***EXECUTOR_NUMBER*** NODE_NAME NODE_LABELS
BUILD_URL JOB_URL

### multibranch 
BRANCH_NAME CHANGE_ID CHANGE_URL CHANGE_TITLE CHANGE_AUTHOR CHANGE_AUTHOR_DISPLAY_NAME CHANGE_AUTHOR_EMAIL CHANGE_TARGET
## params

## currentBuild
### writable properties
result displayName description ***keepLog***
### time related
timeInMillis startTimeInMillis duration durationString
### Other builds
previousBuild nextBuild upstreamBuilds 
### Projected related
projectName fullProjectName
### build related
description ***id*** number currentResult resultIsBetterOrEqualTo(String) resultIsWorseOrEqualTo(String) displayName fullDisplayName 
### scm related
changeSets

### Other
rawBuild https://javadoc.jenkins-ci.org/hudson/model/Run.html

## scm
