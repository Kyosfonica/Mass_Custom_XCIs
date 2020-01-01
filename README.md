# Mass Custom XCI Creator

This program will mass create all possible single base custom XCIs from a NSZ folder that you provide. It will add all updates and dlc that it can find into the XCI. It will keep a database of what it has created, and upon future runs of the program will create any new XCIs from whatever new updates or dlc you had added to the folder. The previous XCI will be deleted assuming it is still in the output folder.

I would like to add XCZ support in the future but for now on only XCI files will be supported.

## NSCB already makes XCI, why did you make this?

You can consider this an extension of what NSCB does. It actually uses the same backbone that NSCB does to create the XCI, squirrel.py. NSCB requires constant manual intervention, you have to feed it files and delete the old XCI. This program automates that manual intervention. After initial setup you can set create.py to be run daily via task scheduler or cron, and never worry about creating them again.

## Setup and Usage

Requires python, and python in PATH.

Requires a keys.txt placed inside of ztools. Obtain this elsewhere.

If you do not already use NSCB, then inside of the ztools folder there is an install dependencies bat. Run that. 

On first run it will ask you for the location of the NSZ root folder. This folder must have a "base" "dlc" and "updates" or "updates (1)" folder. It will also ask if you would like to create an up to date database so that only new files added to the NSP folder will be created, or if you would like to create all XCIs from scratch. 

On future runs, its as simple as running create.py.

## Linux, Mac, and python command not found

If you use mac or linux, you can run the following command to install the squirrel dependencies rather than the included bat made by julesontheroad.
 - `pip install urllib3 unidecode tqdm bs4 tqdm requests image`

If 'pip' or 'python' as commands do not work, you must customize the program to your own usage. Maybe pip3. On line 6 of create.py, set your python command.

## This code is by no means perfect

I am not a python expert so bugs might appear and good practices might not be followed.

This project allows me to save a lot of time by automating a boring task and at the same time I learn some python. 

## Credits

ItsCinnabar for the first Mass XCI creator this project is forked from. https://github.com/ItsCinnabar/Mass_Custom_XCIs

julesontheroad for squirrel, and by extension everyone credited on NSCB's github. https://github.com/julesontheroad/NSC_BUILDER