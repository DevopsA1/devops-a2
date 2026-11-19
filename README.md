# clone main repo, build image from docker file, 
# run container
# to build image
git clone https://github.com/DevopsA1/devops-a2.git
cd devops-a2
docker build -t mahmad29rbq/readerhaven-final:v2.0 .

docker run -d -p 8081:80 --name readerhaven-main mahmad29rbq/readerhaven-final:v2.0