# SigWiz #

SigWiz is a Uniface support utility providing features not yet within the standard Uniface IDE. It's primary focus is the discovery, manipulation, and validation of Uniface signatures relating to COM and 3GL interface. Due to the diverse options interfacing to these non-uniface technologies it can be confusing decoding calls and parameter types.

## Dependencies ##

SigWiz has been written and tested with:

 * Uniface 9.7.01
 * SQLite
  
 ## Setup ##

This project can be downloaded and setup standalone.

### Setup SigWiz as a standalone project ###
These instructions allow you to create a new stand alone project on your local machine.

 * For these steps you'll need the Project Setup Tool. Follow the instructions here https://github.com/uniface/Development-Tooling/tree/master/uniface-project-setup-tool to setup this tool before continuing
 * Clone the SigWiz repository onto your local machine. For these steps we'll assume it's been cloned into C:\Projects\SigWiz
 * Open a command prompt in the root of the project and type "projectsetup97" to invoke the Project Setup Tool
 * Work through the setup process checking the details picked up by the setup tool make sense. Ignore referencies to userid and password they are not used.
 * When complete click on one of the presentation links
  
## Contributing to the project ##

To set up the project for development follow the steps above to create uOutlook as a standalone project. Once complete the only other tool required is the Version Control project, allowing granular exports of source code suitable for use with BitBucket. To set this up follow these steps:

 * Visit https://github.com/uniface/Development-Tooling/tree/master/uniface-version-control and follow the setup instructions to download the Version Control tool
 * Open the IDE and using the Utilities->Import menu import the file FILESYNC_Menu.xml. Assuming you extracted the Version Control tool to C:\\UnifacePackages, this would be found in C:\\UnifacePackages\\VersionControl\\imports
 * Compile the additional menu, which will in turn compile the menu we just imported
 * In the IDE go to Utilities->Preferences->General and tick the check box "Enable Additional Menu"
 * Now that the additional menu is enabled we can go to Utilities->Additional->Settings and using the browse button next to "Uniface Source Directory" select ./src. This points the tool at our source code.
 * Everything is now setup and we can go to Utilities->Additional->Project to verify that everything is setup correctly. Visiting this screen will sync your Uniface repository with the src folder. If it's working correctly then you should see the contents of this folder in the tree view.

## Sample signatures ##

Under exports you can find two export files with some sample C and COM call-out signatures. You can import them into SigWiz from the Tools->Import menu.

## Contributors ##
* Daniel Iseli
* George Mockford
