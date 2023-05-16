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

Ansile playbook configaration managemnet 

To start with, I set up the environment by provisioning a Vagrant virtual machine with the latest Ubuntu Server. I followed the configurations we learned in the course material, where no authentication keys or certificates were needed. For simplicity, I used Jeff Geerling's Ubuntu 20.04, which we had already downloaded and set up.

Next, I created the playbook for the project and placed it in the root directory of my main project. In this playbook, I utilized various concepts to enhance its functionality and maintainability. I defined variables to make the playbook more flexible and reusable. I also used variable files for better organization, which could earn me bonus points. Additionally, I implemented roles to handle different tasks. For instance, I had a role dedicated to front-end logic and containerization. To improve the playbook's readability and ease of assessment, I made use of blocks and tags.

I worked with a GitHub repository that contained the same web app yolomy we worked on in week 2 of this module. The repository's README file listed the components of the yolomy app, which I considered when defining the tasks in my playbook. Each component had its own unique role in the playbook, ensuring clear separation and configurability.

In the playbook, I included tasks that set up Docker containers for the identified components. By doing this, I leveraged the benefits of containerization and managed each container's configuration individually through its role.

Once the playbook was complete, I used it to clone the code from the GitHub repository and run the necessary setups in the Vagrant virtual machine. This ensured the successful execution of the application, which I verified in the browser.

It's worth noting that the project had already been bootstrapped, meaning that following the instructions in the README file automatically launched the application in the browser after running the playbooks successfully.

As part of the requirements, I needed to test the "Add Product" functionality. This feature allowed me to add a product through a provided form, testing the capability to load retail products onto the website. Ensuring the proper functioning of this functionality was crucial for the final deliverable of the assignment.