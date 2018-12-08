# difference
## ARG
only for docker build  
可以通过RUN echo ${HELLO} 输出  
The ARG instruction defines a variable that users can pass at build-time to the builder with the docker build command using the --build-arg <varname>=<value> flag  
  
## ENV
for both docker build and run time docker run xxx -it bash  
可以通过RUN echo ${HELLO} 输出  
The ENV instruction sets the environment variable <key> to the value <value>. This value will be in the environment for all subsequent instructions in the build stage and can be replaced inline in many as well.
  
## LABEL
不可以通过RUN echo ${HELLO} 输出  

