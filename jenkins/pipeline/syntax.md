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
    - always
    - changed
    - fixed
    - regression
    - aborted
    - failure
    - success
    - unstable
    - unsuccessful
    - cleanup

  - stages
  - stage
  - steps
    - script



