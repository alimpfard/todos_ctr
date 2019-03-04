# Todos!

Because clearly every language requires a todo implementation!

### commands

+ add [+priority] \<text\>  
	add a todo entry
+ remove \<idx\>            
	remove an entry
+ resolve \<idx\>
	resolve a todo, but don't remove it
+ unresolve \<idx\>
	reverse of resolve
+ list                    
	list the current todos
+ display                 
	alias for list
+ commit                  
	flush into save (automatically done at exit)
+ help                    
	show the help
+ git \<command\>
	Execute git commands in the save directory
+ import \<url\>
	Import a git url \[Warning: will remove the old data\]
### CLI usage

`executable_name [command] [arguments] [options]`

e.g.
```sh
$ main.ctr add +2 Publish this thing on github

$ main.ctr
```

### config

It will try to read a config file at /etc/ctodo.json or ~/.config/ctodo.json (user dir first)
said config can contain:

+ kill-if-unlucky : there will be an option where the program will refuse to exit, and kill its parent with itself
+ kill-wait : the number of seconds the program will wait before committing murder+suicide

if the config doesn't exist, these default to Nil
