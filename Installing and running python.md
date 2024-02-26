
## Installing Python Means 
<p align="justify">Python installation on a PC involves downloading the Python interpreter and setting up the necessary environment variables. Underneath the hood, the installer extracts files, configures paths, and registers Python in the system, enabling users to execute Python scripts and run applications seamlessly.
</p>
![[Pasted image 20240219180625.png| 500]]
___


# Installing 3rd party packages : 


pip: Package Installer for Python → installing 3rd party libraries (packages) basically requires copying files into the Python installation (whichever directory you want) can be done manually, but again, tedious instead can use another app that is installed alongside Python pip → easily install, update and remove packages uses the Python Package Index https://pypi.org official 3rd party repository for Python.


# Creating Virtual Environment : 
![[Pasted image 20240225194440.png]]
![[Pasted image 20240225195642.png]]
![[Pasted image 20240226105826.png]]
## When you create and activate a virtual environment in Python, several things happen within your computer's file system and **environment**:

  
When you create and activate a virtual environment using tools like `virtualenv` or `venv`, they set the path variable automatically by manipulating the `PATH` environment variable. Here's a breakdown of the process:

1. **Creation of the Virtual Environment**:
    
    - When you create a virtual environment using `virtualenv` or `venv`, a new directory is created containing a self-contained Python interpreter, as well as a copy of the Python standard library and any other packages you install within the virtual environment.
    - Along with the Python interpreter and the standard library, there's also a `bin` directory (on Unix-like systems such as Linux or macOS) or a `Scripts` directory (on Windows) inside the virtual environment directory. This directory contains executable scripts and commands associated with the virtual environment.
2. **Activation of the Virtual Environment**:
    
    - When you activate the virtual environment, the activation script within the `bin` or `Scripts` directory is executed. This script manipulates the environment variables, including the `PATH`.
    - The activation script modifies the `PATH` variable to ensure that when you run Python or any other command, the version of Python and the packages installed in the virtual environment are prioritized over the system-wide ones.
    - It does so by adding the `bin` or `Scripts` directory of the virtual environment to the beginning of the `PATH` variable. This ensures that when you type a command like `python`, the shell finds and executes the version of Python within the virtual environment rather than the system-wide one.
3. **Deactivation of the Virtual Environment**:
    
    - When you deactivate the virtual environment, the activation script reverts the changes it made to the environment variables, including resetting the `PATH` variable to its original state before the virtual environment was activated.
    - This ensures that once you deactivate the virtual environment, any subsequent commands use the system-wide Python interpreter and packages.

By manipulating the `PATH` variable in this way, virtual environments enable you to isolate dependencies for different projects and ensure that they don't interfere with each other or with the system-wide Python installation.

After we activate the virtual environment. it has set the environment variable to the path of our current <font color="#c0504d">Python 12</font> directory.
![[Pasted image 20240226110130.png]]
![[Pasted image 20240226111252.png]]
