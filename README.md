# Project 
### Title
	Config handler module
### Created by
	Joostens Tomek
### Description
	Class to interface easily with config files 

# Download modules
	pip install configparser

# Module usage
### 1. Download module 
	git clone https://github.com/Tomekske/Module_ConfigHandler
### 2. Extract project
### 3. Move ConfigHandler.py script to your project location
### 4. Move test_ConfigHandler.py script to your project location

# Test module
### Option 1
	python test_ConfigHandler.py
### Option 2
	python -W ignore test_ConfigHandler.py 

# Example Reading from config file
### Import module
	from ConfigHandler import Config
### Create object, section and option parameters are required
	c = Config('Default',Default)
### Optionally add as the second parameter the absolute path to the config file
	c = Config('Default',Default,'C://absolute/path/to/config.ini')
### Print data
	print(c.data)

# Example Reading to config file
### Import module
	from ConfigHandler import Config
### Create object, section and option parameters are required
	c = Config()
### Optionally add as the parameter the absolute path to the config file
	c = Config(C://absolute/path/to/config.ini')
### Get data from the config file
	print(c.readData('section','option')
### Write data to config file
	c.writeData('section','option','data')