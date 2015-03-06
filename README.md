# PhpStorm-LiveTemplates
Collections of PhpStorm-LiveTemplates

## Installation

First, find your configuration folder.

	Windows: <your home directory>\.WebIde<version>\config
	Linux: ~\.WebIde<version>\config
	MacOS: ~/Library/Preferences/WebIde<version>

On my MacOS, it would be `~/Library/Preferences/WebIde80` so you have to adjust commands to your platform. There is a `templates/` directory. It contains XML files with Live Templates.

Create a git repository in the `templates/` dir and pull the templates
```bash
$ cd ~/Library/Preferences/WebIde80/templates
$ git init
$ git remote add origin git@github.com:laravel-china/PhpStorm-LiveTemplates.git
$ git pull origin master
```
If this wouldn't work, you should just backup your templates, clone the repo and merge them manually.
