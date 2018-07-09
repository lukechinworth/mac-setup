# Mac Setup

## Apps
* Chrome
    * Sign in to get bookmarks and data
* Firefox
* iTerm
* Spectacle
* Caffeine
* Flycut
* F.lux
* Cyberduck
* Postman
* Sign in for configs
* Robo3T
* Sequel pro
* Vscode
* Sourcetree
* Skype
* Spotify
* Tizen studio
* virtualbox
* Color Picker
    * open `Script Editor`
    * enter text `choose color`
    * save as name: `Color Picker`, format: `Application`
    * add [developer color picker](https://download.panic.com/picker/)

## Software
* Homebrew
```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
* Homebrew services
```sh
brew services
```
should install `homebrew/services` tap. so you can run `brew services start <x>`
* Oh my zsh
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
* Nvm (node version manager)
```sh
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh | bash
```
* Ansible
```sh
sudo easy_install pip
sudo pip install ansible
```
* MongoDB
```sh
brew install mongodb

# start
brew services start mongodb
```
* MySQL
```sh
brew install mysql
# start
brew services start mysql
```
* `rvm`
```sh
\curl -sSL https://get.rvm.io | bash -s stable --ruby
```
* `bundler`
```sh
gem install bundler
```
* [JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html) (java development kit)
* [Vagrant](https://www.vagrantup.com/downloads.html)

## Files
* Private/public key pair
* Hosts file
* Robomongo config
* Sequel pro config

## Settings
* Use zsh as default shell
```sh
chsh -s $(which zsh)
```
* Make all hidden files visible in finder:
```
defaults write com.apple.finder AppleShowAllFiles -boolean true
killall Finder
```
* Save ssh key to keychain so you don't have to enter password after each login:
```sh
ssh-add -K ~/.ssh/id_rsa
```
* Save screenshots to folder instead of desktop:
```sh
mkdir ~/Screenshots
defaults write com.apple.screencapture location ~/Screenshots
```
