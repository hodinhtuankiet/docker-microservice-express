Dowload Oracal VM Virtual Box 
https://drive.google.com/file/d/1z8UWyqm1u4KDPn68hxcbo3QVLrJBwZP7/view
Command tells you where you stand : pwd
Create new folder : mkdir tuankietdev
mount -t vboxsf ShareFilesDocker /root/tuankietdev
copy all file : copy -a tuankietdev/ . final/ ̣(copy file in folder tuankietdev to folder final)
RUN DOCKER : service docker start
docker compose -f 22.txt -p tuankietdev 
