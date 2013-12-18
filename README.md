Plugins to Minepeon is made easy with the new api that's added

### How to use Menu api.
1. make a .xml file inside /plugins/api_menu that look like this:
```
<?xml version="1.0" encoding="ISO-8859-1"?>
<api>
<Menu_text>[your plugin menu text]</Menu_text>
<pl_folder>[your plugin Plugin index file or folder]</pl_folder>
</api>
```
2. fill in Menu_text and pl_folder

### How make "plugin.yml" file
1. make a "plugin.yml" (it have to be named "plugin.yml"!) that look like this:
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

### How to make it work with web installer
1. Compress all files to tar.gz file
2. see example to see how this tar.gz looks like
