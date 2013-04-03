# Dust #

(c) actraiser/Dustlayer

Dustlayer WHQ: http://dustlayer.com
Contact: actraiser@dustlayer.com

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
- C64 Project Skeletons
	- Generate new ASM or BASIC project from Skeletons
		- Preconfigured Projects with BASIC Loader
		- Follows Dustlayer project layout
			- Runs and Compiles without modifications
			- Tutorials on dustlayer.com follow the layout conventions

## Installation ##

Install node.js from [nodejs.org](http://nodejs.org/download/) for your operating system. Then install *dust* via the node package manager

	sudo npm install -g dust

Then you are good to go, typical you want to clone the tools, set them up and start a first project.

	cd ~
	dust clone
	cd dust-osx-setup
	dust setup

	[... once this is done ...]

	dust test # shows if everything is in place


 Then create for example a new 6502 ASM project into the directory myFirstProject. You can choose from preconfigured skeletons which are listed when you execute the command. 

 	cd ~
	dust create asm myProject # creates a new asm project from a template

	cd myProject
	dust compile # compiles the C64 code and runs it in the C64 Emulator


Checkout http://dustlayer.com for tutorials and an indepth explanation how all that stuff works.

From time to time the tool repository is upgraded with new versions or additional tools. The following commands will update your dust executable and the cloned repository. Aftewards you can restart the installation progress.

	cd ~/dust-osx-setup
	dust update
	dust setup # updates everything or installs whats missing

## Next Features ## 

- Compatibility Windows/Linux
- Tighter integration with Vice/Debugging
- More skeletons to choose from
- Additional tools to ease C64 development


