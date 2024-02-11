```markdown
# AirBnB Clone - The Console

## Introduction
The console is the first segment of the AirBnB project at Holberton School that collectively covers fundamental concepts of higher-level programming. The goal of the AirBnB project is to eventually deploy our server as a simple copy of the AirBnB Website (HBnB). A command interpreter is created in this segment to manage objects for the AirBnB (HBnB) website.

## Functionalities of the Command Interpreter:
- Create a new object (e.g., a new User or a new Place)
- Retrieve an object from a file, a database, etc.
- Perform operations on objects (count, compute stats, etc.)
- Update attributes of an object
- Destroy an object

## Table of Contents
1. [Environment](#environment)
2. [Installation](#installation)
3. [File Descriptions](#file-descriptions)
4. [Usage](#usage)
5. [Examples of Use](#examples-of-use)
6. [Bugs](#bugs)
7. [Author](#author)
8. [License](#license)

## Environment
This project is interpreted/tested on Ubuntu 14.04 LTS using Python 3 (version 3.4.3).

## Installation
1. Clone this repository: `git clone https://github.com/Infrixxx/AirBnB_clone_v4`
2. Access the AirBnB directory: `cd AirBnB_clone_v4`
3. Run the console interactively: `./console` and enter commands
4. Run the console non-interactively: `echo "<command>" | ./console.py`

## File Descriptions
- `console.py` - The console contains the entry point of the command interpreter.
- `models/` directory contains classes used for this project.
- `models/engine` directory contains the File Storage class that handles JSON serialization and deserialization.

## Usage
List of commands this console currently supports:
- `EOF` - exits console
- `quit` - exits console
- `<emptyline>` - overwrites default empty line method and does nothing
- `create` - Creates a new instance of `BaseModel`, saves it (to the JSON file) and prints the id
- `destroy` - Deletes an instance based on the class name and id (save the change into the JSON file).
- `show` - Prints the string representation of an instance based on the class name and id.
- `all` - Prints all string representations of all instances based or not on the class name.
- `update` - Updates an instance based on the class name and id by adding or updating attribute (save the change into the JSON file).

## Examples of Use
```bash
vagrantAirBnB_clone$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  create  destroy  help  quit  show  update

(hbnb) all MyModel
** class doesn't exist **
(hbnb) create BaseModel
7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) all BaseModel
[[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}]
(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}
(hbnb) destroy BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
** no instance found **
(hbnb) quit
```

## Bugs
No known bugs at this time.

## Author
BC Rachoshi - [GitHub](https://github.com/Infrixxx) / [Twitter](https://twitter.com/infrixxx)

## License
Public Domain. No copyright protection.
```

Feel free to copy and use this README for your project.
