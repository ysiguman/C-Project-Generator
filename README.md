C-Project-Generator
===================

A plug-in for Sublime-Text 3 which allows the creation and management of C projects.


##Install C Projects Generator :
Clone or [download](https://github.com/ysiguman/C-Project-Generator/archive/master.zip) git repo into your packages folder ( `CTRL + Shift + P` + _browse package_ ) with the name : `C Projects Generator` .
##Create a Make file :

###Condition:
The project must have this file hierarchy:


#####Project\_Folder/ #####
*  __Source/__ 
 *  _Folder which contain sources files_
 * _Ex.: file1.c_
 * _file2.c_
*  __Header/__
*  __Objects/__



Open  Command Palette ( in windows: `CTRL+Shift+P` ) and  execute `Generate Make`.
This command will create the file `makefile.in` at the root of the project here: `Project Folder/`.

##Create a New C Project :
Open  Command Palette ( in windows: `CTRL+Shift+P` ) and  execute `Create C Project`. C Projects created by this command are optimised to work with the command: `Generate Make` of this plug-in.

An input box will appear on the bottom of Sublime, just give a name to your project and choose the folder of his creation.

####File hierarchy of the new project :####


#####Name\_of\_the\_Project/ #####
*  __Source/__ 
 *  'Name of the Project.c'
*  __Header/__
*  __Objects/__


#### Start folder for choose project location :####
By default the start folder in the navigation panel is the USER path ( `C:/Users/Name` for windows, `/home/Name` for linux ). If you have a specific location where you want to save your project without the need each time to return by the navigation panel, you just have to create `Data.sublime-setting` in the data folder of _C Project Generator_ ( `CTRL + Shift + P` on windows execute `browse package` and find the folder of _C Project Generator_ ) and write it with ( Replace FOLDER by the folder you want to ) :

	{
		"folder": "FOLDER"
	}
	
	
__Example :__<br />
If I want to start at : `C:/Users/MyName/Documents/Projects` I must put:


	{
		"folder": "C:/Users/MyName/Documents/Projects"
	}
	

