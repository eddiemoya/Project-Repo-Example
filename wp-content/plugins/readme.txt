To add a new plugin use the following git command:

> git submodule add --name <plugin_name> <repo_uri> wp-content/plugins/<plugin_folder_name>

<plugin_name> 	- 	This is used as a shorthand to refer to submodules so that you can later refer 
			to them this way instead of via the full path - recommend using same value as
			that of <plugin_folder_name>.
<repo_uri>    	- 	This should be the SSH URI (looks like git@domain/repo.git) when this is an 
			internally developed plugin. HTTP URI's are the least preferred.
<plugin_folder_name> -	This is the name of the folder the plugin will reside in, no leading or trailing 
			slashes. NOTE: Some plugins (poorly written ones) may require its containing 
			folder be named a certain way.

This file is necessary in order to force git to track the /wp-content/plugins folder without actually having
any plugins in it.
