# Linux post installations steps
Setup steps after a fresh linux install

## General

`sudo apt install git zsh tmux htop vim curl nnn -y`

**TLP - For laptop's battery saving**

`sudo apt install tlp -Y`

**Liquorix Kernel**

```
sudo add-apt-repository ppa:damentz/liquorix && sudo apt-get update
sudo apt-get install linux-image-liquorix-amd64 linux-headers-liquorix-amd64
```

**Grub Theme**

`wget -O - https://github.com/shvchk/poly-dark/raw/master/install.sh | bash`

## terminal tools

**prezto**
https://github.com/sorin-ionescu/prezto

**oh-my-zsh**

 `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
 
**oh-my-zsh autocomplete**

 Clone this repository into $ZSH_CUSTOM/plugins (by default ~/.oh-my-zsh/custom/plugins)

`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

Add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc):

`plugins=(zsh-autosuggestions)`

**spacevim**
curl -sLf https://spacevim.org/install.sh | bash

**Better cat, find and grep**
https://github.com/sharkdp/bat
https://github.com/sharkdp/fd
https://github.com/BurntSushi/ripgrep

## Code

**vscodium**

```
wget -qO - https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/raw/master/pub.gpg | sudo apt-key add -
echo 'deb https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/raw/repos/debs/ vscodium main' | sudo tee --append /etc/apt/sources.list.d/vscodium.list
sudo apt update && sudo apt install codium
```

**nim**

`curl https://nim-lang.org/choosenim/init.sh -sSf | sh`

**JetBrains idea**

https://www.jetbrains.com/toolbox-app/

## Other software

**Flameshot - screenshot software**

https://github.com/lupoDharkael/flameshot

**Peek - Record gifs**

https://github.com/phw/peek

**Drawing - MS Paint alternative**

https://github.com/maoschanz/drawing

**Timeshift - System back-ups**

```
sudo apt-add-repository -y ppa:teejee2008/ppa
sudo apt-get update
sudo apt-get install timeshift
```

**Spotify**

```
curl -sS https://download.spotify.com/debian/pubkey.gpg | sudo apt-key add - 
echo "deb http://repository.spotify.com stable non-free" | sudo tee /etc/apt/sources.list.d/spotify.list
sudo apt-get update && sudo apt-get install spotify-client
```

**Ulauncher**

https://ulauncher.io/#Download

**Slack**

https://slack.com/intl/en-gb/downloads/linux

**MS Teams**

https://products.office.com/en-us/microsoft-teams/group-chat-software#desktopAppDownloadregion


