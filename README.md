# Introduction 

Hello and welcome to this class on model deployment! We will be going through the process of understanding how model deployment works, basics of container technology, how models are served in production environments and help you deploy your first deep learning web application. Below are some pre-requisites for you to go through that will help us conduct the class in a smooth manner. Make sure to go through the steps and setup your machine. Happy Coding!


# Pre-Requisites 

### 1. Git 

Git is a version controlling tool that helps track changes in code, collaborative development and many other advantages. For now we need git just for the sake of getting this repo on your machine. For now, we need git only for cloning the repository to your machine.

1. Install git from https://git-scm.com/downloads.

2. Clone this repository to your machine using
            
            git clone https://github.com/ChetanTayal138/Model-Deployment.git

### 2. Anaconda 

First things first, lets help you create an isolated environment with all project requirements. This will prevent conflicts between different dependencies between different projects on your machine, letting you create projects in a controlled manner. My preferred environment manager for deep learning projects is conda.

1. Install anaconda from https://docs.anaconda.com/anaconda/install/ 

    a) Windows : https://docs.anaconda.com/anaconda/install/windows/
    
    b) Mac : https://docs.anaconda.com/anaconda/install/mac-os/
    
    c) Linux : https://docs.anaconda.com/anaconda/install/linux/

2. Check the version of your conda version to make sure it was properly installed.

                    conda --version

3. Generally if you wanted to create a new conda environment with python-3.7, flask and tensorflow you could use the following command `conda create -n 'your-env-name' python=3.7 tensorflow flask`. Another way is to make use of a yaml file which will create the environment for you. It uses the dependencies mentioned in the yaml file to create the environment. The `environment.yaml` file in this repository corresponds to this configuration file. Run the following command to create the environment.

                    conda env create -f environment.yml

4. Activate the conda environment using 
            
                    conda activate 'your-env-name'

5. Run the python shell and import tensorflow. If you are able to import tensorflow without any problems, that means everything is working perfectly and we are good to go. 

![verification_image](https://github.com/ChetanTayal138/Model-Deployment/blob/master/images/verify_tensorflow.png)

### 3. Docker

Docker is used for creating containers that allows us to package an application and all ofits dependencies into one place. This allows us to build a piece of software on one machine and run that piece of software in any machine, without typically worrying about what hardware/firmware/OS is being utilized by the machine running the container. 

You can install docker on your machine by following the guide here : https://docs.docker.com/get-docker/

