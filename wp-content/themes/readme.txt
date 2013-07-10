To add a new theme use the following git command:

> git submodule add --name <theme_name> <repo_uri> wp-content/plugins/<theme_folder_name>

<theme_name>   	-   	This is used as a shorthand to refer to submodules so that you can later refer
                      	to them this way instead of via the full path - recommend using same value as
                      	that of <theme_folder_name>.
<repo_uri>      -    	This should be the SSH URI (looks like git@domain/repo.git) when this is an
                        internally developed plugin. HTTP URI's are the least preferred.
<theme_folder_name> -  	This is the name of the folder the theme will reside in, no leading or trailing
                        slashes. NOTE: Some themes & plugins (poorly written ones) may require its containing
                        folder be named a certain way.

This file is necessary in order to force git to track the /wp-content/plugins folder without actually having
any plugins in it.
