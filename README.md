# Config ozsh on Mac M1

## Requirements

- Sdkman
- Ozsh
- Typora

## Customize

```sh
# Install required fonts
brew tap homebrew/cask-fonts
brew cask install font-hack-nerd-font
# Install lsd
brew install lsd
# Install sdkman
```

Change font on "Terminal > Preferences > Profiles > Text" to "Hack Regular Nerd Font Complete Mono 11"

## Configuration

```sh
## Set zsh as default shell
sudo sh -c "echo $(which zsh) >> /etc/shells"
chsh -s $(which zsh)

## Copy custom-theme
cp themes/custom-theme.zsh-theme ~/.oh-my-zsh/themes
cp .zshrc ~/.oh-my-zsh

## Refresh ozsh
source ~/.zshrc
```

## Screenshots

![ss-1](./docs/img/ss-1.png)

![ss-2](./docs/img/ss-2.png)
