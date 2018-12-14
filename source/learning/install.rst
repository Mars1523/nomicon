Installation and Configuration
===========
Basic install guide for the varied resources you'll find yourselves needing to install to develop and deploy code for the robot.

Disclaimer
+++++++

If you're confident enough with Python-related resources, you'll still need to use the same libraries, but feel free to use whatever IDE you want, and skip the Conda section.  
If not, please follow the instructions contained in the Conda section, as it'll make future troubleshooting much less painful.

Installing and Configuring Anaconda
+++++++
Installing Anaconda is very easy. Simply go `here <https://www.anaconda.com/download/>`_
and download the Python 3 version. When the installer prompts you to install Visual Studio Code,please do so. It'll make tasks that you have to do in the future much,much easier.
Now that you've installed Anaconda (your package manager),it's time for you to install your deps.

Open the anaconda prompt and type

conda install -c conda-forge pyhamcrest

Once you're done with that,type

conda install -c conda-forge twisted

What you've just installed are dependencies for the 
