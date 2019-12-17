# streamlit_docker_test

from:

https://maelfabien.github.io/project/Streamlit/#




docker build -f Dockerfile -t app:latest .

docker run -p 8501:8501 app:latest

  test with  dockerslim :

wget https://downloads.dockerslim.com/releases/1.26.1/dist_linux.tar.gz

tar -xvzf dist_linux.tar.gz

./dist_linux/docker-slim build app

docker run -p 8501:8501 app.slim:latest   <--- not working   ?????

$ docker images
REPOSITORY                TAG                 IMAGE ID            CREATED             SIZE
app.slim                  latest              60fd3e0b2a63        5 minutes ago       198MB
docker-slim-empty-image   latest              4149efe18f37        6 minutes ago       0B
app                       latest              51a6377ad8ed        12 minutes ago      1.35GB
