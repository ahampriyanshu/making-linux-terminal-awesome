# Making Linux Terminal Awesome

### [Zsh](https://www.zsh.org/)

> The Z-shell or Zsh is an UNIX shell with support for various plugins and themes.

```sh
sudo apt install zsh      [ Debian/Ubuntu ]
sudo yum install zsh      [ RedHat/CentOS ]
sudo pacman -S zsh        [ Arch/Manjaro ]
sudo dnf install zsh      [ Fedora ]
sudo zypper install zsh   [ OpenSUSE ]
```

![1](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/1.png)

### [Oh My Zsh](https://ohmyz.sh/)

> Oh My Zsh is an open source and community-driven framework for managing Zsh configuration.

* Using curl 
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
* Using wget
```
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

![2](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/2.png)

### Nerd Fonts

> Nerd Fonts is a project that patches developer targeted fonts with a high number of glyphs (icons)

* Download [hack](https://github.com/ryanoasis/nerd-fonts/blob/master/patched-fonts/Hack/Regular/complete/Hack%20Regular%20Nerd%20Font%20Complete.ttf) font and install it by double clicking on the **.tff** file. You can also use any other font but make sure it supports all the icons and glyphs required by **powerlevel10k**.
* Select ``Hack Font`` as the default font.

![3](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/3.png)

### [Powerlevel10k](https://github.com/romkatv/powerlevel10k)

> Powerlevel10k is a theme for Zsh. It emphasizes speed, flexibility and out-of-the-box experience.

```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k
```

![1](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/1.gif)

* By default, an installation prompt will begin, but if it doesn't run ``p10k configure``.
* Change the default theme to ``ZSH_THEME="powerlevel10k/powerlevel10k"`` inside ``~/.zshrc ``.
* Commit the changes by running ``source ~/.zshrc``

![2](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/2.gif)

### [zsh-autosuggestions](https://github.com/marlonrichert/zsh-autosuggestions)

> Real-time type-ahead completion for Zsh. Asynchronous find-as-you-type autocompletion.

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

* Add ``zsh-autocomplete`` to the list of plugins inside ~/.zshrc ``plugins=( [plugins...])``
* Commit the changes by running ``source ~/.zshrc``

![3](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/3.gif)

### [zsh-syntaxhighlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

> This package provides syntax highlighting for the shell zsh. It enables highlighting of commands whilst they are typed at a zsh prompt into an interactive terminal. This helps in reviewing commands before running them, particularly in catching syntax errors.

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

* Add ``zsh-syntax-highlighting`` to the list of plugins inside ~/.zshrc ``plugins=( [plugins...])``
* Commit the changes by running ``source ~/.zshrc``

![4](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/4.gif)



### [fzf](https://github.com/junegunn/fzf)

>It's an interactive Unix filter for command-line that can be used with any list; files, command history, processes, hostnames, bookmarks, git commits, etc.

```
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
```

![5](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/5.gif)

* ``ctrl + t`` to navigate through the file system.

![6](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/6.gif)

* ``ctrl + r`` to navigate through older commands.

![7](https://github.com/ahampriyanshu/making-linux-terminal-awesome/raw/metadata/7.gif)

## If you use VS Code

* Paste this into ``setting.json`` to render all the glyphs-icons in the integrated-terminal.
```
{
"terminal.integrated.fontFamily": "Hack Nerd Font",
"terminal.integrated.shell.osx": "/bin/zsh",
"terminal.integrated.rendererType": "canvas",
"terminal.integrated.lineHeight": 1.3,
}
```
 
## To use ``bash`` again

* For a single session : ``bash``
* To make bash the default terminal : `` chsh -s $(which bash) ``

### Copyright Guidelines
* I will also soon be publishing this article on [GeeksforGeeks](https://www.geeksforgeeks.org/)
