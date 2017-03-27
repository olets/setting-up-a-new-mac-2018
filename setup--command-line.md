# Setting up a new computer

## Command Line

- Xcode tools, Homebrew, ruby with rbenv, git and set up github, node with nvm, yarn, mysql + postgres: in a [separate doc](starting-command-line-tools.md) copied from documentation by [ten1seven](https://github.com/ten1seven) and [greypants](https://github.com/greypants)

	- after installing postgres, either set it up to automatically run:
		```
		brew services start postgresql
		```
		
		or, if you just want to run it manually, add an alias an alias to the too-long-to-remember command to your shell profile:
		
		```
		echo 'alias pgstart="pg_ctl -D /usr/local/var/postgres -l /usr/local/var/postgres/server.log start"' >> ~/.bash_profile
		```
		
		(or install zsh, below, and add the alias to your zsh profile by replacing the end of that command with `>> ~/.bash_profile`)
		

	- Make [Sublime Text's command line tool](http://www.sublimetext.com/docs/3/osx_command_line.html) available:
		
		```
		ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl
		```
		
	- With `npm` installed, install [`npm-check-updates`](https://github.com/tjunnone/npm-check-updates):
	
		```
		npm install -g npm-check-updates
		```

<!--
-To load `.bashrc` and `.profile` in every new terminal, add them to the `.bash_profile`. Listing this last because I've read you "usually" want it at the end of your `.bash_profile`… but that's all I know about that :)

	```
	echo 'source ~/.bashrc' >> ~/.bash_profile
	echo 'source ~/.profile' >> ~/.bash_profile
	```
-->

## Terminal
	
- **zsh** shell + **oh-my-zsh**

	Why? Read [this slide deck with some reasons](https://news.ycombinator.com/item?id=5690235), and ["Comparison of command shells"](https://en.wikipedia.org/wiki/Comparison_of_command_shells)

	- [Docs for installing ZSH](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH) (following the Homebrew instructions is recommended). As of this writing:

		1. Install zsh with

				brew install zsh zsh-completions
		
		1. Give your shell setup access to zsh

				sudo nano /etc/shells
		
			and add `/usr/local/bin/zsh` to the end of the file, and write out.
		1. Set zsh as the default shell

				chsh -s /usr/local/bin/zsh
				
		1. Open a new terminal, and go through the zsh setup

	- [Docs for installing oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
			
	- If you've made any changes to your `~/.bashrc` file, copy over those lines to your `~/.zshrc` file after you switch

	- Add this script ([source](https://github.com/creationix/nvm#deeper-shell-integration)) to `~/.zshrc` to detect and autorun `.nvmrc` files

		```
		# Audodetect nvmrc files
		autoload -U add-zsh-hook
		load-nvmrc() {
		  local node_version="$(nvm version)"
		  local nvmrc_path="$(nvm_find_nvmrc)"
		
		  if [ -n "$nvmrc_path" ]; then
		    local nvmrc_node_version=$(nvm version "$(cat "${nvmrc_path}")")
		
		    if [ "$nvmrc_node_version" != "N/A" ] && [ "$nvmrc_node_version" != "$node_version" ]; then
		      nvm install
		    fi
		  elif [ "$node_version" != "$(nvm version default)" ]; then
		    echo "Reverting to nvm default version"
		    nvm use default
		  fi
		}
		add-zsh-hook chpwd load-nvmrc
		load-nvmrc
		```
	