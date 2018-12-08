# ADD
## Description
The ADD instruction copies new files, directories or remote file URLs from &lt;src&gt; and adds them to the filesystem of the image at the path &lt;dest&gt;.

# COPY
## Description
The COPY instruction copies new files or directories from &lt;src&gt; and adds them to the filesystem of the container at the path &lt;dest&gt;.

# COPY vs ADD
They do some operations, copy files to images. 
ADD 多做了些事情，比如会通过URL下载文件和解压缩压缩文件。
https://www.ctl.io/developers/blog/post/dockerfile-add-vs-copy/ 

 
