# Deploying a Deep Learning model with FastAPI
 
## Introduction
 
This tutorial is specifically designed to run locally on your machine. This can be done via using `Python Virtual Environments`. 
 
Both approaches should yield the same result. If you already have a conda installation available on your computer, we recommend  that you use the virtual environment method. If this is not the case, choose the Docker method as it is easier to set up.
 
As a general note, the commands in this tutorial are meant to be run within a terminal. To begin you need to **clone this repo in your local filesystem and `cd` to the Yolo3-FastAPI
.

To clone the repo use this command:
```bash
git clone https://github.com/jeapsilva/Deploying_MachineLearning_Models.git
```

or for cloning via SSH use:
```bash
git clone https://github.com/jeapsilva/Deploying_MachineLearning_Models.git
```

The `cd` command allows you to change directories. Assuming you are at the directory where you issued the cloning command, type the following on your terminal.
```bash
cd Yolov3-FastAPI
```
This will bring you to the `week1-ungraded-lab` directory. The `ls` command allows you to list the files and directories.
Type `ls` and let's take a quick look at the content inside `week1-ungraded-lab` directory:
 
```
.
└── Yolov3-FastAPI (this directory)
    ├── images (includes some images from ImageNet)
    ├── server.ipynb 
    ├── client.ipynb
    └── requirements.txt (python dependencies)
```
 
 
## Method 1: Python Virtual Environment with Conda
 
### Prerequisites: Have [conda](https://docs.conda.io/en/latest/) installed on your local machine.
 
You will use Conda as an environment management system so that all the dependencies you need for this ungraded lab are stored in an isolated environment.
 
Conda includes a lot of libraries so if you are only installing it to complete this lab , we suggest using [miniconda](https://docs.conda.io/en/latest/miniconda.html), which is a minimal version of conda.
 
### 1. Creating a virtual Environment
 
Now we assume that you either successfully installed conda or that it was previously available in your system. The first step is  creating a new developing environment. Let's set a new environment with python 3.8 with this command:
 
```bash
conda create --name mlops-yolofastapi python=3.8
```
 
After successfully creating the environment, you need to activate it by issuing this command:
 
```bash
conda activate mlops-yolofastapi
```
 
At this point, you will do all your libraries installation and work in this environment. So, whenever working on this ungraded lab, check the mlep-w1-lab environment is active.

 
### 2. Installing dependencies using PIP 
 
Before proceeding, double check that you are currently on the `Yolov3-FastAPI` directory, which includes the `requirements.txt` file. This file lists all the required dependencies and their respective versions. 

Now use the following command to install the required dependencies:
 
```bash
pip install -r requirements.txt
```
 
This command can take a while to run depending on the speed of your internet connection. Once this step completes you should be ready to spin up jupyter lab and begin working on the ungraded lab.
 
### 3. Launching Jupyter Lab
 
Jupyter lab was installed during the previous step so you can launch it with this command:
```bash
jupyter lab
```

### 4. Running the notebook
 
Within Jupyter lab you should be in the same directory where you used the `jupyter lab` command.
 
Look for the `server.ipynb` file and open it to begin.

To stop jupyter lab once you are done with the lab just press `Ctrl + C` twice.
