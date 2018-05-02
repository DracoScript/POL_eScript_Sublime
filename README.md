# POL_eScript_Sublime
Syntax Highlighting + Build for POL eScript in Sublime-Text 3 based on POLeScriptNPP (for Notepad++).

# Installing

??/Sublime-Text-3/Packages/ folder can be found within Sublime-Text-3 -> Preferences -> Browse Packages...

SYNTAX:
To use this syntax highlight on Sublime-Text 3 you must locate your ??/Sublime-Text-3/Packages/ folder and place the .sublime-syntax files inside, usually in the Users folder.
Now when opening .src, .inc and .cfg file they may be pointed to the corresponding POL eScript syntax. If not, you must check your bottom right corner of the sublime window and select from the list (check inside the User or the name of the folder you placed the files within Packages folder).
I used it in a different folder inside Packages folder, named POLServer so I can find both syntaxes inside a submenu named POLServer within the syntax list. ??/Sublime-Text-3/Packages/POLServer/*everything cloned from this git

BUILD:
Recently a build option was inserted and a new file was introduced in order to make it work, it is the .sublime-build file.
This file also goes within any folder inside ??/Sublime-Text-3/Packages/ folder in your computer to work.
This file uses a path based on the first opened folder inside Sublime-Text, which must be the pol folder containing the ecompile.exe file inside the scripts folder. The path is "$folder\scripts\ecompile.exe" and you may change it to match your preferences.
There is a main build command to be ran we used the "Build" inside a file opened with the syntax, because it uses a base scope of source.polscript. This build option may be used using the menu Tools > Build or using the shortcut "Ctrl+B" (for windows).
Within the build file there is a variant for to build all files and it can be accessed using the menu Tools > Build With... or using the shortcut "Ctrl+Shift+B" and selecting the "POL_eScript - Build All" option, since the "POL_eScript" option is the normal functionality of building the current file.

# How can you help?
You may help improve this syntax highlighting by pointing out errors or suggesting new features.
I don't know if there is a way to run the ecompile.exe using linux or osx system, therefore they were not yet added to the build options.
