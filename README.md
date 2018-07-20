# Todos!

Because clearly every language requires a todo implementation!

### commands

+ add [+priority] <text>  
	add a todo entry
+ remove <idx>            
	remove an entry
+ list                    
	list the current todos
+ display                 
	alias for list
+ commit                  
	flush into save (automatically done at exit)
+ help                    
	show the help

### CLI usage

`executable_name [command] [arguments] [options]`

e.g.
```sh
$ main.ctr add +2 Publish this thing on github

$ main.ctr
```
