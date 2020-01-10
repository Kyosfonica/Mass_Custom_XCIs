# Automatic XCI Generator

The main purpose of the this tool is to automatically generate Custom XCI files from previously own NSZ files.
The program will automatically check for base, updates and dlc folders and will generate an XCI file for each titleid it founds.

Once the main database is built, the tool is able to detect file changes and generate a new XCI file if needed.

This program will mass create all possible XCI files based on the NSP folder provided. Create a folder with the files you really want to 
convert to XCI if you do not want them all.

I plan to add XCZ support once it is ready.

# I already have NSBC, why I need this?

If you plan to mass convert NSZ files and do not want to do it by hand then this tool is for you. It will automate the boring stuff
and you will be free to enjoy your time.

If you are only creating a few Custom XCI files from time to time then stay with NSCB as that tool is awesome and it does a lot of stuff this one doesn't.

# Setup

Requires python and python in PATH.

Requires a keys.txt file placed inside the ztools folder. Obtain it elsewhere.

# Usage

On first run the tool will ask you for the location of the NSZ root folder.
This folder must have a "base" "dlc" and "updates" or "updates (1)" folder.

It will also ask if you would like to create an up to date database so that only new files added to the NSP folder will be created,
or if you would like to create all XCIs from scratch.

I recommend the first option as this will keep track of new files or updates for you. 

On future runs, it is as simple as running create.py or create_xci.bat.

# Linux & Mac support

Not right now. Currently this program works on Windows 64bits only.

The reason is because I face a lot of issues installing the dependencies of squirrel on my own computer and I want this tool to work out of the box.

# Credits

ItsCinnabar for the first Mass XCI creator. This project is a fork of it. https://github.com/ItsCinnabar/Mass_Custom_XCIs

julesontheroad for squirrel, and by extension everyone credited on NSCB's github. https://github.com/julesontheroad/NSC_BUILDER

Without squirrel this project would not be possible.