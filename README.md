# concon
Bash Script to backup your Steam(deck) Controller Configurations

Search for steam controller config files in sub-directories, and copy them."
Usage: concon --list <Config-Dir> ..."
       concon [--more|--templates|--all] [--out=<Output-Dir>] [--template-update] [--template-dir=<Template-Dir>] <Config-Dir> ...
Options:
       --help             this!
       --list             only list possible config files
       --quiet            no logging
       --more             use configs not assigned to games
       --template         use templates
       --all              use configs from community
       --template-list    list what would be updated in templates folder
       --template-update  !!! modify template folder !!!
       --template-dir=    use as template folder
       --out=             Output folder (def: ./MyConfigs)
       --log=             Output logfile
 !!! without --out ./MyConfigs will be overwritten !!!

This script is intended to be run on the SteamDeck in a Terminal Window.

Example:
First try: ./concon --list
this will do no harm :-)

Example:
./concon --template-list
This will create a sub directory "MyConfigs" and list all configs which are currently actually used by you for games.
"MyConfig" will be a backup of !!!all!!! your Configs


For naming it relies on SteamCMD-AppID-List, which is included here as a sample. You should use the latest from https://github.com/dgibbs64/SteamCMD-AppID-List for best results.
 
