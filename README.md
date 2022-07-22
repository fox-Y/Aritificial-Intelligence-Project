# Aritificial-Intelligence-Project
## Quick Start
To try out the simulator, install the code on a UNIX system (or a system that has the 'make' program installed and a C++ compiler). Type 'make' to build the 'wumpsim' executable. Then, type './wumpsim'. You should see a randomly-generated 4x4 world, information about the game state, and a prompt for the next action. When the game is over, scoring information is provided.

If you want to code your agent in Python, see the "Python Agent" section below.
## Python Agent
You can also implement your agent in Python 2 or 3. First, you will need to compile a different version of the simulator that supports calling external Python agent functions. Instead of 'make' or 'make wumpsim', you should instead compile the simulator using 'make pywumpsim'. On some platforms you need to set the PYTHONPATH environment variable to your working directory, where pywumpsim and Agent.py reside.

Next, you will make all your changes to the Agent.py file. This file contains the Agent class consisting five methods: constructor (__init__), destructor (__del__), Initialize, Process, and GameOver. Note that the Process method takes a percept class as defined in Percept.py. The Process function should return one of the six actions defined in Action.py.

Once you've finished your Agent.py file, simply run the 'pywumpsim' program to test your agent. The Agent.py file and the 'pywumpsim' executable must be in the same directory. The 'pywumpsim' program accepts all the options described above for 'wumpsim'. And there is no need to recompile 'pywumpsim' after changes to Agent.py; this file is reloaded everytime 'pywumpsim' is executed.
