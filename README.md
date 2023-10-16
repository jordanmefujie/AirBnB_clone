0x00. AirBnB clone - The console


This project is the first step towards building
a full web application: the AirBnB clone.

The console or command interpreter create the data
model and allows create, update, destroy, store and
persist objects to a file(JSON file).
This console will be a tool to validate this storage engine.

Table of Contents
---
* Objetives
* Requeriments
* Installation and execution
* Console commands
* Tests
* Development environment
* Authors

Objectives
---
* How to create a Python package
* How to create a command interpreter in Python using the cmd module
* What is Unit testing and how to implement it in a large project
* How to serialize and deserialize a Class
* How to write and read a JSON file
* How to manage datetime
* What is an UUID
* What is *args and how to use it
* What is **kwargs and how to use it
* How to handle named arguments in a function

Requeriments 📋
---
Airbnb was built and tested in Ubuntu 14.04 LTS via
Vagrant in VirtualBox. Programming languaje python3

Installation and execution 🔧
---
* Clone the repository
* Move in to the directory
> $ cd AirBnB_clone
* Execute the console file
> AirBnB_clone$ ./console.py

Console commands
---
The commands available for this command interpreter are:
	Name/Description
|**create*| Creates a new instance
of the class passed by argument.
|*show*| Prints the string representation of an instance.
|**destroy*| Deletes an instance that was already created.
|*all*| Prints string representation of
all instances or of all instances of a specified classs.
|**update*| Updates an instance attribute if exists otherwise create it.
|*help*| Show all commands or display information about a specific command.
|*quit*| Exit the console.
|*EOF*| Exit the console.

**create, destroy and update commands save changes into a JSON file.*

Commands usage
*Command*/*Usage*
|*create*/**create*** < class_name > (ctrl + d)

Tests

Interactive Mode

Example 1: Using create, count and all commands

$ ./console.py
(hbnb) help

Documented commands (type help < topic >):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$

Example 2: Using basic update with an Id and show command

(hbnb) update BaseModel

Example 3: Using update with a dictionary

(hbnb) BaseModel.update

Example 4: Using destroy and count command

(hbnb) BaseModel.destroy("99f01e9a-99c0-42af-8c10-c35cadee1d8f")
(hbnb) all
(hbnb) BaseModel.count()
0
(hbnb) quit
solid@DESKTOP-6PPFSAT:~/H/AirBnB_clone$

Non - Interactive Mode

solid@DESKTOP-6PPFSAT:~/H/AirBnB_clone$ echo "help" | ./console.py
(hbnb)

Documented commands (type help < topic >):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help < topic >):
========================================
EOF  help  quit
(hbnb) 
$
Development environment
This project has been tested on Ubuntu 14.06.6 LTS

* Programming languaje Python
* The tests are carried out in virtualBox
* Development environment manager vagrant
