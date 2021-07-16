# Mac Setup

## Files to save before wiping old mac

* Private/public key pair
* Hosts file
* Sequel pro config
* Transfer Authy account to another device.

## Apps

* Chrome
  * Sign in to get bookmarks and data
* iTerm
* Spectacle
* Caffeine
* Flycut
* F.lux
* Postman
  * Sign in for configs
* Sequel pro
* Visual Studio Code
  * `cmd` + `P`, enter `> install`, select `Shell command: Install 'code' command in PATH`
* Spotify
* virtualbox
* Visual Studio for Mac
* SquidMan: `brew cask install squidman`
* OmniDiskSweeper: https://www.omnigroup.com/more
* Xcode
* Android Studio
* Cakebrew
* Authy desktop
* Gas Mask
* hide.me
* Local (wp containers)
* Zoom
* Loom
* Paintbrush

## Software

* Xcode command line tools: `xcode-select --install`
* Homebrew
  * If homebrew is giving you permission errors, do: `sudo chown -R $(whoami) $(brew --prefix)/*`
* Homebrew services
* Oh my zsh
* powerlevel10k (instant prompt)
* nvm (node version manager)
  * Set default node version with: `nvm alias default <version>`
* Ansible
* JDK (java development kit)
* vagrant: https://www.vagrantup.com/downloads.html

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
* System Preferences
  * Keyboard
    * Key Repeat: Fast
    * Delay Until Repeat: Short
  * Spotlight
    * Search results: Uncheck all except Applications, Documents, PDF Documents, and Spreadsheets
    * Privacy: Add ~/Development, ~/Virtualbox\ VMs
