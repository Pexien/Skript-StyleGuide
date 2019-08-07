# Skript Style-guide
Skript is a simple way to add functionality to your bukkit based Minecraft server, it does this in the form of multiple scripts which are independently executed; however, it becomes hard to organize and follow a specific format in which maintains an organized structure, and an easy to follow format for someone to view, who is external to the project.

This style-guide creates a format, which will allow you to create clean, semantic scripts that can be easily followed by an individual either external, or internal to a development project, as well as make debugging and scrubbing over the code simpler, and appear to be more comprehensive.

### Table of Contents
[Skript Configuration](##Skript-Configuration) - How to set up the server-side skript configuration file

## Skript Configuration
Skript holds a whole assortment of options which you can change in the skript configuration file which you can use to make your scripts more dynamic and hold better integrity. The `config.sk` file is the script file which contains these options, you can find the configuration file by going to the `./plugins/Skript/config.sk` file within your server's root directory.
> You can reload the configuration file using `/sk reload config`

Once you are within the `config.sk` file, some options you should change for use on any production server are the following:

 - Set the `use player UUIDs in variable names:` option to `true` *(if you are creating a script for a party external to your server, use `%player's uuid%` and `%uuid of player%` if necessarily.)*
 - Set `plugin priority:` to `highest` *(only if skript is your main form of development)*
 - Set `enable timings:` to `true` *(only if you are using paper spigot)*
 
 Thees options ensure that skript always uses a player's uuid as opposed to their player name so that player's changing their named do not have any adverse side effects, and the others are merely troubleshooting and best practices.
