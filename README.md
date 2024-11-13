
# OpenSim installation instructions

These instructions should be replicated if participating in the Opensim research.


## Installation for C++

•	Open sim website

	SimTK: OpenSim: Project Home
•	Access the GitHub repository

•	Under C++ development, click build instructions
 
•	Go to Linux build instructions, we will come back to this.

•	On a separate window open your aws access portal and login to the appropriate user

•	Navigate to EC2 and go to instances on the left hand side  
•	We will be creating an instance for C++ as well as python separately. We will work with C++ first

•	In the top right, click launch instance to create a new instance 

•	You may name the instance whatever you like, just make sure you are able to recognize what the instance will be used for

•	Under Application and OS Images, choose ubuntu but makes sure the version is compatible with the opensim build instructions 

•	The default will be 24.04, but we want 22.04
 
•	Change the instance type to t2.2xlarge 

•	Key pair should be opensim_key 

•	Change storage to 128 

•	Now we may launch the instance

•	Now we can go back to our terminal. You must have ubuntu 22.04 installed on your computer

•	Type ubuntu in the terminal and it should launch 

•	To connect to aws, go to the aws browser and click on your instance, it should be highlighted. At the top of the screen click the connect button 

•	Copy the example for ssh client and paste that into your terminal. Make sure to type yes and enter when prompted 

•	You are now connected to aws

•	Type ‘sudo apt upgrade’ and when that is done type ‘sudo apt update’ type y and enter when prompted

•	Going back to the linux build instructions, click the link  

•	Once on the page, we want to click on raw and copy the browser link and type ‘wget raw.githubusercontent.com/opensim-org/opensim-core/refs/heads/main/scripts/build/opensim-core-linux-build-script.sh’ into your terminal 
 
•	We will now have this download. To check, type ‘ls’ into the terminal
•	We want to follow the build instructions for linux on the github page

## Installation for Python

•	Use the same steps to connect to python instance 

•	Instead of using build instructions for C++, go to scripting in conda and click conda package.

•	To be able to use the conda command, you must first download anaconda onto your terminal.

•	On the page below, copy the link of the x86 python installer for linux 

•	Type wget https://repo.anaconda.com/archive/Anaconda3-2024.06-1-Linux-x86_64.sh

•	If you cannot get permission use the sudo chmod +x prefix to the file name

•	Follow the instructions for the download

•	When prompted, type yes and then restart the shell for changes to take effect

•	conda install -c conda-forge python=3.11




    