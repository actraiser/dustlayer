# Dust #

(c) actraiser/Dustlayer

Dustlayer WHQ: http://dustlayer.com
Contact: actraiser@dustlayer.com

Dust is part of a bigger project consisting of a blog with coding tutorials and various projects. Check the Website.

## Synopsis ##

Dust ist a node.js driven versatile command line suite for new and experienced C64 programmers on Mac OSX. 
This first version installs and configures the tool chain and helps you to kickstart cross-development projects. 

## Feature List ##

- Cross Development Setup Installer
	- Installs and configures all tools required for efficient C64 Coding (currently only OSX)
		- ACME
		- Vice
		- Crunchers
		- and more
	- Automatic Sublime Installation and Configuration
		- 6502 and BASIC syntax highlighting
		- Instangt Build & Run Options for ASM and BASIC projects
		- Auto-Start in Vice via BASIC loader
- Advanced Vice integration
	- Labels export to Vice Monitor at Build time
	- Compile and Run in Vice from Editor
- C64 Coding Tutorials
	- Generate new ASM or BASIC project from Tutorials Database
		- Preconfigured Projects with BASIC Loader
		- Follows Dustlayer project layout
			- Runs and Compiles without modifications

## Installation ##

Install node.js from [nodejs.org](http://nodejs.org/download/) for your operating system. Then install *dust* via the node package manager

	sudo npm install -g dustlayer

Then you are good to go, typical you want to setup the tools:

	dust setup

	[... once this is done ...]

	dust test # shows if everything is in place


 Download a tutorial to check if your setup works: 

 	cd ~
	dust tutorials # list tutorial code and select one for download
	# cd into the directory and run dust compile	
	dust compile # compiles the C64 code and runs it in the C64 Emulator

or open the project in Sublime first and build from context menu 

 	# cd into the directory 
 	sublime .

Then hit CMD-B - if nothing happens, you need to select one time the appropriate build system in Tools->Build System->C64-6502, then hit again CMD-B

Checkout http://dustlayer.com for tutorials and an indepth explanation how all that stuff works.

-act/Dustlayer
