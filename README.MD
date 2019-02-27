This repository contains methods to Dockerize Python Projects.

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
     ![image](https://user-images.githubusercontent.com/689226/53516344-175d5500-3af2-11e9-9f23-feddbd3135c8.png)
     Before executing the below commands, I preffered to clean the docker history. Followed the below commands:
      - docker rm -vf $(docker ps -a -q)
      - docker rmi -f $(docker images -a -q) 
     ![image](https://user-images.githubusercontent.com/689226/53516510-80dd6380-3af2-11e9-8f07-09f3bf07bc82.png)
   * Check Docker Hub: [[Docker Hub URL]](https://hub.docker.com/r/rahulvaish/flaskwebservicedocker/)
     ![image](https://user-images.githubusercontent.com/689226/49725174-181fe100-fc91-11e8-8900-84403a4a4b9b.png)

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
