# Learning Docker
### Why Docker?
- Docker helps solve the "It works on my machine problem". With Docker, we can codify the resources needed for any app. 
- Dockerfile is used to provide instructions about the resources needed for a particular app and create an Image 
- Image can then be uploaded to Docker Registry and downloaded to another host to create a similar container 
- Since the container is exactly based on the copy, there will not be any issues caused by inconsistency in the underlying resources
- Unlike VMs, containers use the same OS. So no need for extra licensing, patching etc. Containers are isolated process with its own filesystem. They're lightweight and faster as they basically use a process of the OS which is already running

### Linux CLI commands
> echo
> whoami 
> echo $0 
> apt list 
> apt install nano
> apt update
> apt remove nano 
> nano 
> pwd (print working directory) 
> ls -l
> ls -1 
> ls -a
> cd 
> cd .. (one level up) 
> cd ../.. (two levels up) 
> cd ~ (takes to home directory) 
> mkdir newdir
> touch hello.txt 
> touch file1.txt file2.txt file3.txt file4.txt 
> mv fromdir todir 
> mv file1.txt newname.txt 
> rm file1.txt 
> rm  file1.txt file2.txt
> rm file*
> rm -r dirname 
> cat file1.txt 
> more file1.txt 
> less file1.txt 
> head 
> head -n 5 
> tail 
> cat file1.txt > file2.txt 
> grep hello file1.txt 
> grep -i hello file1.txt 
> grep -i hello file*
> grep -ir hello dirname 
> find 
> find -type d 
> find -type f 
> find -type f -name "file*"
> find -type f -iname "file*"
> mkdir test; cd test; echo done 
> mkdir test && cd test && echo done (if a step fails, subsequent steps will not run) 
> mkdir test || echo "directory exists"
> ls /bin | less 
> printenv 
> printenv PATH 
> echo $PATH 
> export DB_USER=mosh
> echo $DB_USER 
> echo DB_USER >> .bashrc 
> source ~/.bashrc (reloads the file) 
> ps 
> kill pid  
> sleep 100 &
> useradd -m john 
> adduser bob
> cat /etc/passwd 
> usermod -s /bin/bash _john_
> cat /etc/passwd
> cat /etc/shadow
> docker exec -it -u _john_ _container_id_ bash 
> userdel john
> groupadd developers 
> cat /etc/group
> usermod -G developers _john_
> groups _john_
> echo echo hello > deploy.sh
> chmod u+x deploy.sh ( - would remove )  

- / is the root directory 
- Root is the home directory for root user and every other directory is inside it 
- bin, boot, dev, etc, home, root, lib, var, proc 
- cd can work with either relative or absolute path. Absolute paths always begin with root 
- Most of the commands are programs in the bin directory 
- Use \ for multiline commands 
- Permissions
- first letter tells  whether file or directory
- next three groups 
- Permissions for the owner of file 
- Permissions for group 
- Permissions for everyone else 

### Docker Hub


### Commands 
> docker pull ubuntu 
> docker run ubuntu 
> docker run -it ubuntu 
> docker ps
> docker ps -a 

### Building Images ###

