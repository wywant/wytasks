# CMD
一个Dockerfile只能有一个CMD

# ENTRYPOINT
Only the last ENTRYPOINT instruction in the Dockerfile will have an effect.



# difference
当docker run后面跟命令的时候， CMD将不会运行， 但是ENTRIPOINT会运行
