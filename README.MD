### To Dockerize a Flask WebService Project. Follow the below steps:
 * Download the FlaskWebServiceDocker project.
 * Navigate inside the FlaskWebServiceDocker project folder from Docker QuickStart Terminal.
 * Execute the below commands-
     ![image](https://user-images.githubusercontent.com/689226/49724797-2d484000-fc90-11e8-94f7-052f4b1a5710.png)
     ![image](https://user-images.githubusercontent.com/689226/49724798-2f120380-fc90-11e8-89b5-f6925cb6e74d.png)
     </br>
     Before executing the below commands, I preffered to clean the docker history. Followed the below commands: </br>
     - docker rm -vf $(docker ps -a -q) </br>
     - docker rmi -f $(docker images -a -q) </br>
      
     ![image](https://user-images.githubusercontent.com/689226/53516344-175d5500-3af2-11e9-9f23-feddbd3135c8.png)
     Here we have used -p which specifies the port it is going to run on. In out Calculator.py file we used app.run(debug=True, host=’0.0.0.0') so we needed to specify which port when using flask run , which above you can see I used 5000. </br>
     
     ![image](https://user-images.githubusercontent.com/689226/53516510-80dd6380-3af2-11e9-8f07-09f3bf07bc82.png)
  * Check Docker Hub: [[Docker Hub URL]](https://hub.docker.com/r/rahulvaish/flaskwebservicedocker/)
     ![image](https://user-images.githubusercontent.com/689226/49725174-181fe100-fc91-11e8-8900-84403a4a4b9b.png)

<hr>

##### [Complete Document](https://github.com/rahulvaish/ReferenceDocuments/blob/master/UnderstandingDocker/StepsToDockerizeFlaskWebServiceProject.docx)

<hr>

##### Reference Repository:
##### [FlaskWebService-Python](https://github.com/rahulvaish/FlaskWebServices-Python)



