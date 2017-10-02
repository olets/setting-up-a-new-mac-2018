# Setting up a new computer

[TOC]

## Command Line Tools

- Follow the [documentation](starting-command-line-tools.md) by from documentation by [ten1seven](https://github.com/ten1seven) and [greypants](https://github.com/greypants) to set up Xcode tools, Homebrew, ruby with rbenv, git and set up github, node with nvm, yarn, mysql + postgres, and then

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

## Homebrew Packages

Some of the packages I use most are

  - [speedtest-cli](https://github.com/sivel/speedtest-cli) - install via Homebrew with `brew install speedtest-cli`
  - [trash-cli](https://github.com/sindresorhus/trash-cli) - install via Homebrew with `brew install trash-cli`
  - [tree](http://mama.indstate.edu/users/ice/tree/) - install via Homebrew with `brew install tree

You can install fonts, including some I use in the terminal and in code editors, with Homebrew. This means you'll get any updates to the fonts!

```shell
brew tap caskroom/fonts
```

Then you can `brew search your-font-name`. You can see the full list of font in the [fonts cask repo](https://github.com/caskroom/homebrew-fonts).

<!--
-To load `.bashrc` and `.profile` in every new terminal, add them to the `.bash_profile`. Listing this last because I've read you "usually" want it at the end of your `.bash_profile`… but that's all I know about that :)

	​```
	echo 'source ~/.bashrc' >> ~/.bash_profile
	echo 'source ~/.profile' >> ~/.bash_profile
	​```
-->

## Terminal

**zsh** shell + **oh-my-zsh**

Why? Read [this slide deck with some reasons](https://news.ycombinator.com/item?id=5690235), and ["Comparison of command shells"](https://en.wikipedia.org/wiki/Comparison_of_command_shells)

- [Docs for installing ZSH](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH) (following the Homebrew instructions is recommended). As of this writing:

  1. Install zsh with

     brew install zsh zsh-completions

  2. Give your shell setup access to zsh

     sudo nano /etc/shells

     and add `/usr/local/bin/zsh` to the end of the file, and write out.
  3. Set zsh as the default shell

     chsh -s /usr/local/bin/zsh

  4. Open a new terminal, and go through the zsh setup

- [Docs for installing oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

- If you've made any changes to your `~/.bashrc` file, copy over those lines to your `~/.zshrc` file after you switch

### (z)shell setup

  - **Autoload the correct version of node via nvm**

    Add this script ([source](https://github.com/creationix/nvm#deeper-shell-integration)) to `~/.zshrc` to detect and autorun `.nvmrc` files

    ```shell
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

  - **A custom terminal window title:**

    ```shell
    # custom window title
    # this will show "cwd (process)"
    set-window-title() {
      window_title="\033]0;${PWD##*/}\007"
      echo -ne "$window_title"
    }
    PR_TITLEBAR=''
    set-window-title
    add-zsh-hook precmd set-window-title
    ```

### oh-my-zsh setup

- **oh-my-zsh options** (edit `~/.zshrc`)

  Uncomment `DISABLE_AUTO_TITLE="true"`

- **oh-my-zsh plugins** (edit `~/.zshrc`)

  ```shell
  plugins=(git emoji colored-man-pages zsh-history-substring-search thefuck zsh-autosuggestions zsh-syntax-highlighting)
  ```

- **Theme**

  [Spaceship](https://github.com/denysdovhan/spaceship-zsh-theme)


  - **Theme options**

    ```shell
    SPACESHIP_GIT_STATUS_INDEX_PREFIX=" [ "
    SPACESHIP_GIT_STATUS_ADDED='added∆s '
    SPACESHIP_GIT_STATUS_MODIFIED='unstaged∆s '
    SPACESHIP_GIT_STATUS_UNTRACKED='untracked∆s '
    SPACESHIP_GIT_STATUS_STASHED='stashed∆s '
    SPACESHIP_GIT_STATUS_BEHIND='behind '
    SPACESHIP_GIT_STATUS_AHEAD='ahead '
    SPACESHIP_TIME_SHOW=true
    SPACESHIP_PACKAGE_SHOW=false
    SPACESHIP_PROMPT_DEFAULT_PREFIX=" "
    SPACESHIP_RUBY_PREFIX=" "
    SPACESHIP_NODE_PREFIX=" "
    SPACESHIP_RUBY_SYMBOL="💎  " # adds an extra space for kerning
    SPACESHIP_EXEC_TIME_SHOW=false
    SPACESHIP_BATTERY_DISCHARGING_SYMBOL="🔌 "
    SPACESHIP_BATTERY_FULL_SYMBOL="🔋 "
    ```
