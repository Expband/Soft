The usual, pre-installed Terminal <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b3/Terminalicon2.png/240px-Terminalicon2.png" alt="terminal mac os logo" height="25" width="25"> application on `Mac OS` has quite limited customization and expansion options. 
There are several themes available to choose from, and downloading third-party ones is quite difficult. 
To solve this problem comes the iTerm2 application. There are many themes to choose from to use with it, you can create your own or 
customize someone else's.<br>
<img src="https://upload.wikimedia.org/wikipedia/commons/3/31/ITerm2_v3.4_icon.png" alt="iTerm2 logo" height="100" width="100"><br>
The Homebrew script is used for downloading: `brew install --cask iterm2`. After installing the terminal itself, 
I install the following extensions:<br>

__oh-my-zsh__ <br>
<img src="https://camo.githubusercontent.com/4db3e4069e59f51d03dd3e7fa5e89ab8fb95c9f4acda36cd5bfdf58d95269d92/68747470733a2f2f6f686d797a73682e73332e616d617a6f6e6177732e636f6d2f6f6d7a2d616e73692d6769746875622e706e67" alt="oh-my-zsh logo" heigth="100" width="100">
- `oh-my-zsh` to improve console interaction. You need to use wget to install the framework. Command to install:<br>
  `sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`<br>
  The framework provides the following plugins:<br>
  - `aliases` adds ability to create shortcuts, pre-installed for tree view(`l, ls, lsa`) and for github(`gaa, gp`)<br>
  - `git` This plugin supports working with GitHub from the command line. It provides configures the hub shell and termination for the git command if you have hub installed, also completion for github ruby stone, and convenience functions for working with repositories and URLs<br>

   And many, many (298) plugins that are immediately available for use. [Documentation](https://github.com/ohmyzsh/ohmyzsh/wiki/)<br>

__zsh-syntax-highlighting__ <br>
<img src="https://avatars.githubusercontent.com/u/567410?s=48&v=4" alt="GitHub Avatar" width="100" height="100">

- `zsh-syntax-highlighting` next on the list, but not least, is to install the syntax highlighting plugin, which helps with writing commands. The main functionality of this plugin is highlighting various types of objects, highlighting them by color, and so on. To use, you need to clone the repository:<br>
```git clone https://github.com/zsh-users/zsh-syntax-highlighting.git```<br>
```echo \"source ${(q-)PWD}/zsh-syntax -highlighting/zsh-syntax-highlighting.zsh\" >> ${ZDOTDIR:-$HOME}/.zshrc```<br>
and create a script using <br>
`source ./zsh-syntax-highlighting/zsh-syntax-highlighting.zsh`<br>
[Documentation](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md)

__zsh-autosuggestions__ <br>
<img src="https://avatars.githubusercontent.com/u/567410?s=48&v=4" alt="GitHub Avatar" width="100" height="100">

- `zsh-autosuggestions` a plug-in that, based on the history of entered commands and the list of available commands, offers quick command entry when pressing the `Tab` button.<br>
[Documentation](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md)

__POWERLEVEL10K__

- a plugin that adds a nice and user-friendly terminal look. With the help of this plugin, you can output to the console the branches you are on while working with git. Working directory path, prompt execution time, UTC time. In addition to good looks, it has a rather important, as for me, functionality. To install plugin put <br>

`git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k`<br>
`echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc`

After executing the echo command, you need to restart the terminal. After opening the terminal, you need to make settings using the configuration wizard. [Documentation](https://github.com/romkatv/powerlevel10k#features)

__.zshrc__ <br>
<img src="https://ih1.redbubble.net/image.3459550440.8279/st,small,507x507-pad,600x600,f8f8f8.jpg" heigth="100" width="100"> <br>

In order to install all plugins, you need to configure the .zshrc configuration file, which is not immediately available. Therefore, first it should be created using the `touch ~/.zshrc` command. Then you need to configure it. But if you like the look of my `terminal` <br>
![my terminal look](../diff/terminal_screen.png)
Copy and use mine. But if you like the look of my terminal, copy and use [`mine`](zshrc.txt). To open it, use the `open ~/.zshrc` command

__Color Presets__ <br>
<img src="https://img-fotki.yandex.ru/get/99813/366311221.85/0_17c07d_e14e54fb_XL.jpg" height="100" width="110"> <br>

Also, as an application, you can set color themes for the terminal. This is done much easier than the previous steps:
  1) Download any color theme you like
  2) Open `iTerm2`, and go to the settings section by pressing `⌘ + ,`
  3) Go to the tab `Profiles` > `Colors`
  4) In the `Color Presets` drop-down list, select `Import` and specify the path to the loaded preset. Restart the terminal and you're done.
I used `[this portal](https://iterm2colorschemes.com/)` to find and download presets.

As an option, you can create your own theme by choosing your shade, transparency, and so on for each color.
