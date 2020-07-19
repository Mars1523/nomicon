Installation and Configuration
==============================

Basic install guide for the varied resources you'll find yourselves needing to
install to develop and deploy code for the robot.

Installing Anaconda
+++++++++++++++++++

Installing Anaconda is very easy. Simply go `here
<https://www.anaconda.com/download/>`__ and download the Python 3 version.
When the installer prompts you to install Visual Studio Code, do so.
Now that you've installed Anaconda, it's time for you to install dependencies.

Open the anaconda prompt and type

.. code:: sh

    conda install -c conda-forge pyhamcrest

Installing RobotPy
++++++++++++++++++

.. note::

    The RobotPy docs explain instalation in more detail
    `here <https://robotpy.readthedocs.io/en/latest/install/pyfrc.html>`__

To install RobotPy run the command:

.. code:: sh

    pip install pyfrc

Now that you've installed PyFRC, there are a few more dependencies to add.
Grab :code:`robotpy-ctre` and :code:`robotpy-navx` with pip.

It's now time to tackle the Tensorflow installation, which requires a bit
more work. unfortunately, Tensorflow does not yet work with Python 3.7, so we
need to work around that.

.. note::

    As soon as Tensorflow supports 3.7, this will no longer be needed.


One would normally assume that TensorFlow could be
installed,like you've installed everything else. However,Tensorflow
doesn't work at all in Python 3.7.  Instead of waiting around for support
to be added soon™, we're going to configure a virtual environment in Conda,
running Python 3.6.7, that will allow us to circumvent that issue.



First off, you'll need to open your Conda command line. Type this command.

.. code:: sh

    conda update conda

Once you've updated conda, type the below to create your virtual environment.

.. code:: sh

    conda create -n (your name for the virtual env here) python=3.6.7 anaconda

Once you've created the virtual environment, you can install tensorflow
inside the virtual environment, like this:

.. code:: sh

    conda activate (your env name here)

And then:

.. tensorflow or tensorflow-gpu?

.. code:: sh

    conda install -n (your name here) tensorflow-gpu

Once you've done that, congrats, you have Conda installed in your virtual
environment. To use it, just manually specify the virtual environment
in VSCode which should be under a file path similar to this.

C:/Users/(your username here)/Anaconda3/envs/(your env name here)/python.exe
​


