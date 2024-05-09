# docker-getting-started-app
Practice Buid & Run , Share Docker 
## Dowload Oracal VM Virtual Box 
`https://drive.google.com/file/d/1z8UWyqm1u4KDPn68hxcbo3QVLrJBwZP7/view ` <br/>
`Command tells you where you stand : pwd` <br/>
`Create new folder : mkdir tuankietdev` <br/>
`mount -t vboxsf ShareFilesDocker /root/tuankietdev` <br/>
`copy all file : copy -a tuankietdev/ . final/ ̣(copy file in folder tuankietdev to folder final)` <br/>
`RUN DOCKER : service docker start` <br/>
`docker compose -f 22.txt -p tuankietdev` <br/>
## Implement With Docker Desktop : https://docs.docker.com/get-started/03_updating_app/
`Build your updated version of the image, using : docker build -t getting-started .` <br/>
Start a new container using the updated code : docker run -dp 3000:3000 getting-started
Container run only one Port <br/>
List image , container : docker ps or docker ps -a  <br/>
You can stop and remove a container in a single command by adding : docker rm -f <the-container-id> <br/>
## Share Image To Docker Hub
`Share docker if u without login Docker Hub : docker push docker/getting-started` <br/>
`If u have an error like this: denied: requested access to the resource is denied
unauthorized: authentication required -> https://docs.docker.com/get-started/04_sharing_app/` <br/>
`Share docker with login Docker Hub : docker push tuankietdev(your-name)/getting-started` <br/> 
`Then error : An image does not exist locally with the tag: tuankietdev/getting-started` <br/> 
`Using solve to authozie repositories after built an Image(getting-started) : docker tag getting-started(name-image) YOUR-USER-NAME/getting-started(name repositories)` <br/> 
`List image on docker : docker image ls `
