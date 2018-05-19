# Project 
### Title
	Config handler module
### Created by
	Joostens Tomek
### Description
	Class to interface easily with config files 
### Version
	1.0.5


# Setup
	python setup.py install


# Test module
### Option 1
	python test_ConfigHandler.py
### Option 2
	python -W ignore test_ConfigHandler.py 


# Example
### Import module
	import ConfigHandler
### Create object, section and option parameters are required
	c = ConfigHandler.Config()
### Optionally add as the parameter the absolute or relative path to the config file
	c = Config(C://absolute/path/to/config.ini')
### Get data from the config file
	print(c.readData('section','option'))
### Write data to the config file
	c.writeData('section','option','data')
### Check if a section in the config file exsists
	print(c.checkSection('section'))
### Check if an option in the config file exsists 
	print(c.checkOption('section','option'))
