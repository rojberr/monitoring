# monitoring

![Photo by Bobby Stevenson on Unsplash](readme-pic.jpg)

k3d cluster create mycluster --agents 3 --api-port 6550
k3d cluster edit mycluster --port-add "30000-32767:30000-32767@server:0"