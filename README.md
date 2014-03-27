docker-mongo
============

creates a docker-container running mongodb with given config-file.

## installation

you do not need to clone this repository - docker does this for you. Just paste this command:

    docker build -t d1rk-mongo github.com/d1rk/docker-mongo
  
You should be able to see your newly created image `d1rk-mongo` in the ouput of docker images:

    docker images
  
Now, you can start a new container using this image like this:

    sudo docker run -name mongodb_ins -d -p 27020:27017 d1rk-mongo
  
There will be a mongodb instance running and listening on port 27020 on your machine.

