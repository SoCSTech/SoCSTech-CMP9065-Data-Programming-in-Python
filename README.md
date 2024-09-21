# CMP9065 - Data Programming in Python
This repository houses the course materials for the Data Programming in Python module at the University of Lincoln. 

In order to set up your personal computer to run the module lectures and workshops' Jupyter Notebooks, you have two options:

 - [Setup with Docker](#setup-with-docker) - this is the same setup you have in the labs PC.
 - [Native setup](#native-setup) - simpler, but may cause conflicts with other packages/softwares already installed.


---
# Setup with Docker
## What is Docker?
Docker is a platform which allows developers to create and share containers.

A container is an environment separate from your main operating system, which includes all of the requirements to run a piece of software. You can think of it like a box which you can take anywhere,
and when opened, the software inside works exactly the same way, no matter where you are running it.

This helps us technicians to give every module the exact coding environment it needs, without causing any conflicts.

If you would like to learn more about how Docker works in your labs, please feel free to contact us at technician@lincoln.ac.uk.

## How do I use the Docker container for this module at home?

We strongly recommend using the Docker container for your modules on your personal devices, as it recreates the exact coding environment you use in the labs without installing lots of stuff on your computer which may conflict with the required software for other modules you are studying.

### Prerequisites

These prerequisites are the same for every Computer Science module using Docker containers, so you should only need to do this once and it will work for the rest of your degree.

1. Download and install Docker Desktop: https://www.docker.com/products/docker-desktop/

2. Download and install VSCode: https://code.visualstudio.com/

3. Install the Remote Development extension for VSCode: https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack

### Process

1. Clone this repository to your computer by opening a command prompt (a.k.a. terminal) and launching
   ```
   git clone https://github.com/SoCSTech/CMP9065-Data-Programming-in-Python.git
   ```
3. Inside the cloned folder, there is a folder entitled **CMP9065 Data Programming in Python** which contains the .devcontainer folder.
4. Make sure Docker Desktop is running. You can minimise the window.
5. Open VS Code, go to **File -> Open Folder**, and select your **CMP9065 Data Programming in Python** folder.
6. Click the **Reopen in container** pop up in the bottom right corner of your VS Code window. If you do not see this pop up, press F1, and type **Reopen in Container**, and click on the **Dev Containers: Reopen in Container** command.
7. The Docker image will now be downloaded, and the container will be started. You can click **show log** in the bottom right corner to see what is going on.
8. Your docker container is now running! Within this VS Code window, you can now run workshop or assignment material exactly the same as in the computing labs.
9. Every week there will be new materials pushed to this repository. In order to get the most up-to-date version of the materials every time, before starting to work open a command prompt inside the **CMP9065-Data-Programming-in-Python** folder and enter
   ```
   git pull
   ```

### Troubleshooting

If you are struggling to get this to work, try these common troubleshooting steps:

1. Restart your computer. Always a good start.
2. Make sure Docker Desktop is open and running.
3. Make sure Docker Desktop is updated.
4. Make sure VS Code has the Remote Development extension pack. You can install this through the Extensions tab in VS Code if it isn't working through the web link above.


# Native setup
Following these steps you will be downloading all the software packages required for this software on your computer. Some packages may conflict with already existing installations, if that is the case (or you are worried it may be the case), we suggest you setup your PC following the [Setup with Docker](#setup-with-docker) instructions.
## Process
1. Ensure you have the latest version of Python installed. It can be obtained from [https://www.python.org/downloads/](https://www.python.org/downloads/) for all operating sytems.
2. Using your Command Prompt/Terminal launch the following command to install Jupyter Notebook
   ```
   pip install --upgrade pip
   pip install notebook
   ```
3. From the command prompt, install all the packages required throughout the module:
   ```
   pip install scikit-learn scikit-image seaborn matplotlib numpy pandas scipy
   ```
1. Clone this repository to your computer by opening a command prompt and launching
   ```
   git clone https://github.com/SoCSTech/CMP9065-Data-Programming-in-Python.git
   ```
3. Now that Python and Jupyter Notebook are installed use Command Prompt/Terminal (or similar) to run the command:​
   ```
   jupyter notebook
   ```
4. The previous step should have opened a browser window at [http://localhost:8888/](http://localhost:8888/), if not go to this address by clicking the link here.
5. Select the folder  **CMP9065-Data-Programming-in-Python/CMP9065 Data Programming in Python** which contains the content of the module you have cloned.
6. Open the notebook file for the corresponding week you need to work on; for example, **Workshop 1 - Module Overview and Introduction to Python.ipynb**.
9. Every week there will be new materials pushed to this repository. In order to get the most up-to-date version of the materials every time, before starting to work open a command prompt inside the **CMP9065-Data-Programming-in-Python** folder and enter
   ```
   git pull
   ```


