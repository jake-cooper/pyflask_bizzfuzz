# Task
Please set up a new project, using python, flask, and Vagrant.

When visiting http://localhost:5000 the app should respond with an html page which includes
bootstrap, and a simple layout to display tabular data with three columns: number, fizz, buzz.
- The table should count from 1 to 100
- if the number is divisible by 3, please display a glyphicon­ok​in the Fizz column
- if it’s divisible by 5, display a glyphicon­ok i​n the Buzz column.
- If it’s divisible by both, both ticks should be displayed, and both should be green.


# How things work
Folder structure

```
  /.vagrant           #
	/templates          # Flask templates  
  app.py              # This file is called by start.sh
	start.sh            # Shell script which starts the Python-Flask web server "http://localhost:5000"
	Vagrantfile         # Provisioned spec of the Vagrant VM.(Requirements file)

```


# Fizz Buzz goes Hello World
The project should include a requirements file to specify python dependencies, and running
'vagrant up​' should produce a working vm with all dependencies installed and
web server can be started by running the following sequence:

1 vagrant up
2 vagrant ssh
3 cd /vagrant
4 ./start.sh


# Some useful insights if using Windows 7
* These points should not be taken as gospel, just a hint if you running Windows 7 and having issues.

- Windows CMD will not let you run 'vagrant ssh' from command line even with Administrator permissions.
- Solution 1: Use PuTTY to SSH into VM
- Solution 2: Install Linux or OS/X
