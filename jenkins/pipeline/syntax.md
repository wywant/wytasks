# Blocks
Blocks must only consist of Sections, Directives, Steps, or assignment statements
# Sections
Sections in Declarative Pipeline typically contain one or more Directives or Steps.
## agent
top level and stage level
## post

# stages
Containing a sequence of one or more stage directives, the stages section is where the bulk of the "work" described by a Pipeline will be located. 

pipeline
  - directive environment
  - directive options
    - buildDiscarder
    - checkoutToSubdirectory
    - disableConcurrentBuilds
    - newContainerPerStage
    - overrideIndexTriggers
    - preserveStashes
    - quietPeriod
    - retry
    - skipDefaultCheckout
    - skipStagesAfterUnstable
    - timeout
    - timestamps
    - parallelsAlwaysFailFast

  - directive parameters
    - string
    - text
    - booleanParam
    - choice
    - file
    - password

  - directive triggers
    - cron
    - pollSCM
    - upstream
  - directive tools
    - maven
    - jdk
    - gradle
  - input
    - message
    - id
    - ok
    - submitter
    - submitterParameter
    - parameters

  - section agent

  - section post 
    - condition always
    - condition changed
    - condition fixed
    - condition regression
    - condition aborted
    - condition failure
    - condition success
    - condition unstable
    - condition unsuccessful
    - condition cleanup

  - section stages
    - directive stage
      - when
        - branch
        - buildingTag
        - changelog
        - changeset
        - changeRequest
        - environment
        - equals
        - expression
        - tag
        - not
        - allOf
        - anyOf
        - triggeredBy

      
  - section steps
    - script



