# docker-mongodb

## Getting Started

Get the image via index.docker.io

        $ docker pull networld/mongodb

        or build from source

        $ IMAGE_NAME=networld/mongodb
        $ docker build -rm -t ${IMAGE_NAME} .

Start a container with:

        $ docker run -name mongodb -p 127.0.0.1:27017:27017 -d $IMAGE_NAME

Use mongodb from other container:

        $ docker run -link=mongodb:mongo -i -t ubuntu /bin/bash
        $ echo $MONGO_PORT_5672_TCP_PORT
        $ echo $MONGO_PORT_5672_TCP_ADDR

## License

The Sigimera Copyright (c) 2013 - 2014 by
[Sigimera Ltd.](http://www.sigimera.com)

## Warranty

This software is provided "as is" and without any express or implied
warranties, including, without limitation, the implied warranties of
merchantability and fitness for a particular purpose.
