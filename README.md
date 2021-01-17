# zsh

![main](https://user-images.githubusercontent.com/54521023/104815966-003ac400-583e-11eb-9dfc-4647ba9556b6.gif)

* via curl 
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
* via wget
```
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

# Nerd Font

* Go to [https://github.com/ryanoasis](https://github.com/ryanoasis)
* Download any font you prefer but make sure it support all the icons and characters required by powerlevel10k [hack](https://github.com/ryanoasis/nerd-fonts/blob/master/patched-fonts/Hack/Regular/complete/Hack%20Regular%20Nerd%20Font%20Complete.ttf) is strongly recommended.
* Install the **.tff** file and make ``Hack Font`` the default font of your terminal

# Powerlevel10k

![powerlevel](https://user-images.githubusercontent.com/54521023/104815969-0335b480-583e-11eb-9fba-d46c3ae21f33.gif)

```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k
```
* By default a installation prompt will begin, but if it doesn't use ``p10k configure``. You can use it later also to try all the different themes and options
* Activate powerlevel10k by changing the default theme to ``ZSH_THEME="powerlevel10k/powerlevel10k"`` in ``~/.zshrc``

# zsh-autocomplete

![auto](https://user-images.githubusercontent.com/54521023/104815959-f2853e80-583d-11eb-8846-2d65b4cff9b4.gif)

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
* Add the plugin to the list of plugins inside ~/.zshrc ``plugins=( [plugins...] zsh-autosuggestions)``
* Activate the plugin by ``source ~/.zshrc``

# zsh-syntaxhighlighting

![syntax](https://user-images.githubusercontent.com/54521023/104815970-04ff7800-583e-11eb-9357-eccd3c972617.gif)


```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
* Add the plugin to the list of plugins inside ~/.zshrc ``plugins=( [plugins...] zsh-syntax-highlighting)``
* Activate the plugin by ``source ~/.zshrc``

# fzf

![fzf](https://user-images.githubusercontent.com/54521023/104815961-fa44e300-583d-11eb-83a5-3d8a9866fba0.gif)

```
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
```

* Use ``ctrl + r`` to search for commands
* Use ``ctrl + t`` to search for files

# If you use VS Code

* Paste this into ``setting.json`` 
```
{
"terminal.integrated.fontFamily": "Hack Nerd Font",
"terminal.integrated.shell.osx": "/bin/zsh",
"terminal.integrated.rendererType": "canvas",
"terminal.integrated.lineHeight": 1.3,
}
```
 
# Reset

* To use bash again type ``bash`` in the terminal
* To go back to back to bash terminal type `` chsh -s $(which bash) ``
