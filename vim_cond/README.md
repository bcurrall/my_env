# Vim setup

## Table of Contents
1. [Get vim](#get vim)
2. [Tutorials](#tutorial)

### Acknowledgements
<p>
Created by: Benjamin B. Currall<br>
Created date: 02/19/18<br>
<br>
Last edited by: Benjamin B. Currall<br>
Last edited date: 02/19/18<br>
</p>


## Vim <a name="get vim"></a>

### Get Vim

```sh
$ sudo apt-get vim
```

### Tutorials <a name ="tutorial"></a>

```sh
$ vimtutor
```

#### Vundle Tutorials

[Vundle Tutorial][1]
[Vundle GitHub Repository][2]

## Vundle

get Vundle
```sh
$ git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

## Edit your vimrc

Open your vimrc
```
$ vim ~/.vimrc
```

Write in:
```
set nocompatible
filetype off

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()

" let Vundle manage Vundle, required
Plugin 'VundleVim/Vundle.vim'

" All of your Plugins must be added before the following line
call vundle#end()
filetype plugin indent on
```

Open vim and type
```
:PluginInstall
```




###References and Acknowledgements

This is a modification of a setup tutorial originally made by Tatsiana Anytolik with assistance from Matthew Stone.

[1]: https://www.youtube.com/watch?v=JVpxDuxe1eY
[2]: https://github.com/VundleVim/Vundle.vim
