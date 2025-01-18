# P1 Initial Streaming Project
Name: Adrian Vega
Date: 1/17/2025
Assignment: Project 1

## Overview

This project introduces streaming data. 
The Python language includes generators - we'll use this feature to generate some streaming buzzline messages. 
As the code runs, it will continuously update log file. 
We'll use a consumer to modify this log file and alert us when a special message is detected. 

## Requirements

1. Python 3.11
    - The most current version of Python is 3.13. 
    - This course will use advanced tools (such as Kafka) that still require Python 3.11. 
2. Virtual Enviornment
3. Git
4. IDE (Visual Studio Code)

## Generate Streaming Data (Terminal 1)

Now we'll generate some streaming data using a producer.

Windows PowerShell:

```shell
.venv\Scripts\activate
py -m producers.basic_producer_vega
```

Mac/Linux:
```zsh
source .venv/bin/activate
python3 -m producers.basic_producer_vega
```

## Monitor an Active Log File (Terminal 2)

A common streaming task is monitoring a log file as it is being written. 
This project has a consumer that reads and processes our own log file as log messages arrive. 

In VS Code, open a NEW terminal in your root project folder. 
Use the commands below to activate .venv, and run the file as a module. 

Windows:
```shell
.venv\Scripts\activate
py -m consumers.basic_consumer_vega.py
```

Mac/Linux:
```zsh
source .venv/bin/activate
python3 -m consumers.basic_consumer_vega.py
```

## Save Space
To save disk space, you can delete the .venv folder when not actively working on this project.
We can always recreate it, activate it, and reinstall the necessary packages later. 
Managing Python virtual environments is a necessary and valuable skill. 
We will get a good amount of practice. 

## License
This project is licensed under the MIT License as an example project. 
You are encouraged to fork, copy, explore, and modify the code as you like. 
See the [LICENSE](LICENSE.txt) file for more.
