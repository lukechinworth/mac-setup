# Mac Setup

## Files to save before wiping old mac

* Private/public key pair.
* Transfer Passwords 2fa codes.

## Apps

* Chrome
* Maccy (clipboard mgr)
* Rectangle (window mgr)
* Caffeine
* Postman
* Visual Studio Code
  * `cmd` + `P`, enter `> install`, select `Shell command: Install 'code' command in PATH`
* Local (WP containers)
* Zoom
* Spotify

## Optional

* TablePlus (MySQL GUI)
* OmniDiskSweeper - https://www.omnigroup.com/more
* Xcode - https://developer.apple.com/download/applications/
  * Download from apple downloads page, NOT the Mac App Store.
* Android Studio
* hide.me (VPN)

## Software

* Xcode command line tools: `xcode-select --install`
* Oh my zsh (shell cfg) - https://github.com/ohmyzsh/ohmyzsh
* Homebrew (pkg mgr) - https://github.com/Homebrew/brew/releases
  * If homebrew is giving you permission errors, do: `sudo chown -R $(whoami) $(brew --prefix)/*`
* nvm (node version manager)
  * Set default node version with: `nvm alias default <version>`

## Settings

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

## System Settings
* Keyboard
  * Key Repeat: Fast
  * Delay Until Repeat: Short
* Spotlight
  * Search results: Uncheck all except Applications, Documents, PDF Documents, and Spreadsheets
  * Privacy: Add ~/Development
* Displays
  * Night Shift: Sunrise to sunset, and set color to warmest.
