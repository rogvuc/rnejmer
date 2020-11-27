WHAT IS RNEJMER
-
Rnejmer is batch file renaming tool written in python. It sends file names to any text editor and lets you rename your files from there with all advanced futures that of a text editor (find all, replace all, regex, etc.). This is really early version and it is NOT MEANT for production use or use on important data. FILE DELITON BUGS ARE POSSIBLE

 USAGE
-
Basically you just point rnejmer to a folder with files you want to rename and it will give you a list of files in that folder in a text editor ready for renaming, if path is not given it will use a current working directory. Rnejmer by default uses whatever text editor is called by editor command in your terminal.

You can modify its behavior with fallowing options:

* -g Try to automatically use default GUI text editor with xdg
* -e < editor_name> choose any editor you want to use
* -v give a more verbose output
	
for example rename all files in a dir foo and be verbose:

	rnejmer -v /dir/path/foo

rename all files in a dir boo using xed editor:
	
	rnejmer -e xed /dir/path/boo

rename all files in a dir bar using default gui editor:

	rnejmer -g /dir/path/bar

INSTALLING
-
#### MANUAL:

1. Install dependency python natsort. You can do that using pip `pip install natsort` or if you are on Ubuntu based distro you can use `apt install python3-natsort`. If you are on some other distro using your package manager is preferred over pip.

2. Download pynamer and copy it to your `/usr/local/bin/` dir
3. Make it executable

#### DEB PACAGE
If you are on Ubuntu or Ubuntu based distro(mint, pop_os, etc..) you can just download and install provided [deb package](https://github.com/rogvuc/rnejmer/releases). It will install rnejmer and take care of a dependency
