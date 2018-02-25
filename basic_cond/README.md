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

Vim
```sh
$ vimtutor
```

TMUX
[Basic tmux Tutorial][4]


#### TMUX

install
```
sudo apt-get install tmux
```

configure setup
add to ~/.tmux.conf
```
set -g mouse on
```

#### Vundle Tutorials

[Vundle Tutorial][1] <br>
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

#### NERDTree

[NERDTree][3]

```
cd ~/.vim/bundle
git clone https://github.com/scrooloose/nerdtree.git
```

Open ~/.vimrc, add to Plugins
```
Plugin 'scrooloose/nerdtree
```

To map quick key, add to .vimrc
```
map <C-n> :NERDTreeToggle<CR>
```

#### Slime

setup
```
cd ~/.vim/bundle
git clone git://github.com/jpalardy/vim-slime.git
```

Open ~/.vimrc, add to Plugins
```
Plugin 'jpalardy/vim-slime
```

Reconfigure to tmux
Open ~/.vimrc, add to defaults
```
let g:slime_taget = "tmux"
```


###References and Acknowledgements

This is a modification of a setup tutorial originally made by Tatsiana Anytolik with assistance from Matthew Stone.

[1]: https://www.youtube.com/watch?v=JVpxDuxe1eY
[2]: https://github.com/VundleVim/Vundle.vim
[3]: https://github.com/scrooloose/nerdtree
[4]: https://www.youtube.com/watch?v=BHhA_ZKjyxo
