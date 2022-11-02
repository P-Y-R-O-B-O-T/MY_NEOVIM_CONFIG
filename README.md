# MY_NEOVIM_CONFIG
My NEOVIM config

* Install powerline fonts
* Install nerd fonts
* Install patch fonts

# Install Powerline Fonts
* Install powerline and fonts using pip using these commands
```sh
sudo apt-get install python3-pip
```
```sh
sudo pip3 install powerline-status
```
```sh
sudo apt-get install fonts-powerline
```
* Enable/Start powerline by adding lines given below at the end of .bashrc file
```sh
# load powerline
if [ -f `which powerline-daemon` ]; then
    powerline-daemon -q
    POWERLINE_BASH_CONTINUATION=1
    POWERLINE_BASH_SELECT=1
fi
if [ -f /usr/local/lib/python3.8/dist-packages/powerline/bindings/bash/powerline.sh ]; then
    source /usr/local/lib/python3.8/dist-packages/powerline/bindings/bash/powerline.sh
fi
```

* Also consider https://github.com/powerline/fonts

# Install Nerd Fonts
* Download nerd fonts from https://www.nerdfonts.com/ and paste ttf(font files) in ./fonts directory of system
* Use webdevicons and ubuntu nerd fonts
