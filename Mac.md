
## Tap to click

https://apple.stackexchange.com/q/382098/452961
https://osxdaily.com/2014/01/31/turn-on-mac-touch-to-click-command-line
https://apple.stackexchange.com/q/353528/452961

```bash
defaults write com.apple.driver.AppleBluetoothMultitouch.trackpad Clicking -bool true
defaults write com.apple.AppleMultitouchTrackpad Clicking -bool true

defaults -currentHost write NSGlobalDomain com.apple.mouse.tapBehavior -int 1
defaults write NSGlobalDomain com.apple.mouse.tapBehavior -int 1

/System/Library/PrivateFrameworks/SystemAdministration.framework/Resources/activateSettings -u
```


Can't agree to terms after iCloud login in setup

https://apple.stackexchange.com/q/362306/452961