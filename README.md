Plugins to Minepeon is made easy with the new api that's added 

Example: [https://github.com/mariogrip/minepeon-plugin](https://github.com/mariogrip/minepeon-plugin)

### How the files gonna be placed inside the install file!

*  http/plugins/[your app foler]/plugin.xml 
*  http/plugins/[your app foler]/uninstal.xml 
*  http/plugins/[your app foler]/uninstal.sh 
*  http/plugins/api_menu/[your app foler]_apimenu.xml 
*  http/instal_temp/instal.xml 
*  http/instal_temp/instal.sh


### How to use Menu api.
1. make a ```[yourappfoldername]_apimenu.xml``` (foldername is the name on the your plugin's folder) file inside /plugins/api_menu that look like this:
```
<?xml version="1.0" encoding="ISO-8859-1"?>
<api>
<Menu_text>[your plugin menu text]</Menu_text>
<pl_folder>[your plugin Plugin index file or folder]</pl_folder>
</api>
```
2. fill in Menu_text and pl_folder

### How make ```plugin.xml``` file
1. make a ```plugin.xml``` (it have to be named ```plugin.xml```!) that look like this:
```
<?xml version="1.0" encoding="ISO-8859-1"?>
<plugin>
<name>[plugin name]</name>
<maker>[your username]</maker>
<description>[Description]</description>
<settings>[settings file]</settings>
</plugin>
```
2. Fill in all fields in the xml file (the settings look like this "plugins/testpl/settings.php")

### instal.xml file
1. make a `instal.xml` file inside /http/instal_temp that look like this:
```
<?xml version="1.0" encoding="ISO-8859-1"?>
<instal>
<run_sh_file>instal.sh</run_sh_file>
<redirect_after>testpl/settings.php</redirect_after>
</instal>
```
If you don't wanna use sh file just write "False", <br>
If you don't need redirect_after or run_sh_file then don't make the instal_temp file

### uninstal.xml
1. make a `uninstal.xml` file inside /http/plugins/[yourappfoler] that look like this:
```
<?xml version="1.0" encoding="ISO-8859-1"?>
<uninstal>
<run_sh_file>uninstal.sh</run_sh_file>
</uninstal>
```
If you don't need this file if you don't have an uninstal.sh file

### How to make it work with web installer
1. Compress all files to tar.gz file
2. see example to see how this tar.gz looks like (example can you find here: [https://github.com/mariogrip/minepeon-plugin](https://github.com/mariogrip/minepeon-plugin))
