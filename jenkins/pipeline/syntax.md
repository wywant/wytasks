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
  - environment
  - options
  - parameters
  - triggers
  - tools

  - agent

  - post 
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

  - stages
  - stage
  - steps
    - script



