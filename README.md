# Development Environment
![Screen Shot 2019-07-03 at 6.38.02 PM.png](https://github.com/Gonzalo8642/DevEnv/blob/master/resources/78C4C939C0DE27CCA6786AC1DAE67CF3.png)

This will guide you through installing my development enviorment. This was written with MacOS in mind but should be available in Windows and Linux with little modifications.

This will go over:
* iTerm2
* Oh My Zsh
* Editors

# Install

## iTerm2

`brew cask install iterm2`
    
Or, if you do not have homebrew [Download](http://www.iterm2.com/downloads.html) and install iTerm2 

iTerm2 has better color fidelity than the built in Terminal, so your themes will look better.
    
Get the iTerm color settings

- [Solarized Dark theme](https://raw.githubusercontent.com/mbadolato/iTerm2-Color-Schemes/master/schemes/Solarized%20Dark%20-%20Patched.itermcolors) (patched version to fix the bright black value)

    
Just save it somewhere and open the file(s). The color settings will be imported into iTerm2. Apply them in iTerm through iTerm → preferences → profiles → colors → load presets. You can create a different profile other than `Default` if you wish to do so.

## Enable Scrolling in Vim 

Scrolling isn't enabled in Vim for iTerm like it is in Terminal. This fixes that.
* iTerm2 > Preferences > Advanced
* Mouse > Scroll wheel sends arrow keys in alternate screen mode > change to yes

## Enable word jumps and word deletion, aka natural text selection

By default, word jumps (option + → or ←) and word deletions (option + backspace) do not work. To enable these, go to "iTerm → Preferences → Profiles → Keys → Load Preset... → Natural Text Editing → Boom! Head explodes".

# Oh My Zsh 

More info here: https://github.com/robbyrussell/oh-my-zsh

## Install with curl
    
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
    
When the installation is done, edit `~/.zshrc` and set `ZSH_THEME="agnoster"` or just use my .zshrc file.



## Install a patched font

- [Source Code Pro](https://github.com/powerline/fonts/blob/master/SourceCodePro/Source%20Code%20Pro%20for%20Powerline.otf) (I use this font @ 14pt)
- [Powerline Font](https://github.com/powerline/fonts) (Or download multiple fonts, this also includes Source Code Pro)
    
Open the downloaded font and press "Install Font".

Set this font in iTerm2 (iTerm → Preferences → Profiles → Text → Change Font), best to do this for "Font" and for "Non-ASCII Font".

Restart iTerm2 for all changes to take effect.


# My Zsh Config
Install instructions can be found in my [zshrc]() repo.

# Editors
I use VS Code as my main editor. Check out my [VSCode+Vim](quiver:///notes/1883F046-004C-43C1-94AA-0A6A9AAAA418) config for more info.

Sometimes it's quicker to edit a file in vim itself. My [vimrc](https://github.com/Gonzalo8642/vimrc) will walk you through the installation.
