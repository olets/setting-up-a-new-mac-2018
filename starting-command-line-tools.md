## Command Line Tools

### install Xcode command line tools
```shell
xcode-select --install
```

### install Homebrew
http://brew.sh/

```shell
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### install Ruby with RBENV
https://github.com/rbenv/rbenv#homebrew-on-mac-os-x

```shell
brew update
brew install rbenv ruby-build
rbenv init
```

### install Git and set up Github account

```shell
brew install git

git config --global user.name "Your Name Here"
git config --global user.email "your_email@example.com"
```

[Add your SSH keys to Github](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/).

### install Node with NVM
https://github.com/creationix/nvm

```shell
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
```

### Install Yarn

https://yarnpkg.com/en/docs/install#mac-tab.

```shell
brew update
brew install yarn
```

Add <code>export PATH="$PATH:`yarn global bin`"</code> to your profile (this may be in your .profile, .bashrc, .zshrc, etc.)

### mysql and postgres databases 

Almost every project uses one of these. Might as well set them up now. Make sure to read the post-install instructions for both to get a username/pass).

```shell
brew install mysql
brew install postgres
```