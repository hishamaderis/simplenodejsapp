# simplenodejsapp
simple node js app, with dockerfile for kubernetes testing

To deploy
1. clone the repository
2. create an image using the Dockerfile
3. push the image to hub.docker.com
4. create deployment: kubectl create deployment hello-node --image=hub.docker.com/repositoryname/hello-node
5. Expose the pod as service: kubectl expose deployment hello-node --type=LoadBalancer --port=8080

