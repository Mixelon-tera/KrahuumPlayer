KrahuumPlayer
==========

Consist of 2 Part

1. You have to mount folder "model: to Docker Server PATH: /opt/models/
(<path_to_model> you have to fill PATH to folder "model" in your computer)

### command to mount folder "model" to "models" in docker Server

docker run -it -p 8080:80 -v <path_to_model>:/opt/models jcsilva/docker-kaldi-gstreamer-server:latest /bin/bash

 2. after that use this command to give the model work (in docker server)

 /opt/start.sh -y /opt/models/sample_nnet2.yaml

 3. open terminal of cmd(if you use window) and go to the K2 PATH and use this command to start server in K2 folder

 http-server -p 8000

 ###you have to install http-server by -> pip install http-server before use above command
# KrahuumPlayer
