frist i test the application on my local environmemt as per the instraction given 
moved in to the client and created a dockerfile 
moved in to backend directory to create a docker file  
I created docker-compose.yml which has mongodb as the servier ,backend container ,client container ,was able to create one network for the containoers to connect
updated my npm to version had an error with the backend not connecting 
edited my  base image to node:20.0.0-alpine3.16 I
changed backend/package-lock.json to state
updated client/serverjs
tested my app by adding an image which worked.
posted yoloclient and yolo backend imgaes to dockerhub which reduced the volume to  64mb and 154.68mb respectivy 