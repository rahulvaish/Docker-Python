This repository contains methods to Dockerize Python Projects.

###### [[Docker Reference Documents]](https://github.com/rahulvaish/ReferenceDocuments/tree/master/UnderstandingDocker)

### Table of Contents
  - <a href='#helloworld-python-docker'>HelloWorld Python Docker</a> 
  - <a href='#flask-webservice-docker'>Flask WebService Docker</a> 
  - <a href='#jupyter-notebook-on-mybinder'>Jupyter Notebook on MyBinder</a> 
  
<hr>

- ###### [HelloWorld Python Docker](https://github.com/rahulvaish/Docker-Python/tree/HelloWorldPythonDocker) 
   ###### This example illustrates how to Dockerize a simple Python Project. [[Source Code]](https://github.com/rahulvaish/Docker-Python/tree/HelloWorldPythonDocker)
   * Download the HelloWorldPythonDocker project.
   * Navigate inside the HelloWorldPythonDocker project folder from Docker QuickStart Terminal.
   * Execute the below commands-
   ![image](https://user-images.githubusercontent.com/689226/50327319-8e83d500-0514-11e9-9f9e-7f04f1680fe9.png)
   ![image](https://user-images.githubusercontent.com/689226/50327517-795b7600-0515-11e9-901e-1348699f7682.png)
   * Check Docker Hub: [[Docker Hub URL]](https://cloud.docker.com/repository/docker/rahulvaish/helloworldpythondocker)
![image](https://user-images.githubusercontent.com/689226/50343937-ec351300-054e-11e9-9a99-9e3fd3daf5c9.png)

 <hr>

- ###### [Flask WebService Docker](https://github.com/rahulvaish/Docker-Python/tree/FlaskWebServiceDocker) 
   ###### This example illustrates how to Dockerize a Flask WebService Project. [[Source Code]](https://github.com/rahulvaish/Docker-Python/tree/FlaskWebServiceDocker)
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
     Here we have used -p which specifies the port it is going to run on. In our Calculator.py file we used app.run(debug=True, host=’0.0.0.0') so we needed to specify which port when using flask run , which above you can see I used 5000. </br>
     ![image](https://user-images.githubusercontent.com/689226/62388441-f4d8d780-b57a-11e9-8e17-0159945d3b9a.png)

    
     <hr>
    
     **FYI:** Refer [[Source Code]](https://github.com/rahulvaish/Docker-Python/tree/FlaskWebServiceDockerAppRoute/FlaskWebServiceDocker-AppRoute) to compute Request/Response like below:
     ![image](https://user-images.githubusercontent.com/689226/62390543-30c26b80-b580-11e9-9b24-91f3016b929d.png)

     <hr>
   
     
   * Check Docker Hub: [[Docker Hub URL]](https://hub.docker.com/r/rahulvaish/flaskwebservicedocker/)
     ![image](https://user-images.githubusercontent.com/689226/49725174-181fe100-fc91-11e8-8900-84403a4a4b9b.png)

   **NOTE: The above service is not meant to be executed on Cloud Environment.** To design the project we need various other components like **gunicorn** which gets dockerize along with the service enabling it to get executed on any Cloud Environment. Follow the below steps:
   
   * Code the Web Service Project  [[Source Code]](https://github.com/rahulvaish/Docker-Python/tree/FlaskWebServiceCloud)
   * Dockerize the Project:</br>
  ![image](https://user-images.githubusercontent.com/689226/54067237-ca048480-4263-11e9-9770-11b9582c7458.png)
  ![image](https://user-images.githubusercontent.com/689226/54067246-ebfe0700-4263-11e9-9226-431f80843b4e.png)
  ![image](https://user-images.githubusercontent.com/689226/54067336-c6253200-4264-11e9-80fb-106f3f119bac.png)
  ![image](https://user-images.githubusercontent.com/689226/54067358-0a183700-4265-11e9-9bdb-590e52ab444c.png)
   * On Azure, Create Resource -> Web -> Web App for Containers <br>
  ![image](https://user-images.githubusercontent.com/689226/54067506-da6a2e80-4266-11e9-9679-d27b8b6a0578.png)
  ![image](https://user-images.githubusercontent.com/689226/54067472-6d569900-4266-11e9-8704-62530b0890e0.png)


<hr>

- ###### [Jupyter Notebook on MyBinder](https://github.com/rahulvaish/Docker-Python/tree/JupyterBinder) 
   ###### This example illustrates how Jupyter Notebooks can be shared on MyBinder which Dockerizes the Notebook under the hood. [[Source Code]](https://github.com/rahulvaish/Docker-Python/tree/JupyterBinder)
   * Open https://mybinder.org/
   * Fill the required fields: </br> 
   ![image](https://user-images.githubusercontent.com/689226/50533889-a503df00-0b59-11e9-8c9d-a58b8fbf0c61.png)
   Notice:In case you want to share your binder link: https://mybinder.org/v2/gh/rahulvaish/Docker-Python/JupyterBinder?filepath=IRIS.ipynb
   * Click Launch  </br>
   ![image](https://user-images.githubusercontent.com/689226/50533795-e4313080-0b57-11e9-93a4-583ed0bc576d.png)
   * FYI: </br>
   ![image](https://user-images.githubusercontent.com/689226/50533883-6110da00-0b59-11e9-8e83-93327bbdd32a.png)
