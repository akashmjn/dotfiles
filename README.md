# Global configuration files 

## BASH: Custom bash profile

## GIT: Git config and ignore files

## VIM: Vim and Bash configurations
My local settings for vim editor and bash/terminal

### How to configure
Follow the following steps to configure your vim and bash
* Clone this repo `$ cd ~ && git clone https://github.com/akashmjn/dotfiles.git` to your home folder.
* Rename the folder to `.vim` or execute this `$ cd ~ && mv dotfiles/ .vim/`
* Take backup of existing .vimrc and .bashrc files, just in case if something goes wrong you can restore them. Follow the following steps to do it,


    ```shell
    $ mv ~/.bashrc ~/.bashrc_backup
    $ mv ~/.vimrc ~/.vimrc_backup
    $ cp ~/.vim/bashrc.vim ~/.bashrc
    $ cp ~/.vim/vimrc.vim ~/.vimrc
    ```


* So the final step is just open you editor `$ vim` and execute this command: `:PluginInstall`.

# Contact me
Email me on [akash7190@gmail.com](mailto:akash7190@gmail.com)
