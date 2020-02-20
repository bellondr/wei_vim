" ----------------vim-go_config_start-----------------------------------------------------------
set nocompatible              " be iMproved, required
set smartcase
autocmd VimEnter * NERDTreeToggle
filetype off                  " required

let g:neocomplete#enable_at_startup = 1
" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
" alternatively, pass a path where Vundle should install plugins
"call vundle#begin('~/some/path/here')

" let Vundle manage Vundle, required
Plugin 'gmarik/Vundle.vim'

" The following are examples of different formats supported.
" Keep Plugin commands between vundle#begin/end.
" plugin on GitHub repo
Plugin 'tpope/vim-fugitive'
" plugin from http://vim-scripts.org/vim/scripts.html
" Plugin 'L9'
" Git plugin not hosted on GitHub
Plugin 'git://git.wincent.com/command-t.git'
" git repos on your local machine (i.e. when working on your own plugin)
" Plugin 'file:///home/gmarik/path/to/plugin'
" The sparkup vim script is in a subdirectory of this repo called vim.
" Pass the path to set the runtimepath properly.
Plugin 'rstacruz/sparkup', {'rtp': 'vim/'}
" Avoid a name conflict with L9
" Plugin 'user/L9', {'name': 'newL9'}

" Install vim-go
Plugin 'fatih/vim-go'
Plugin 'nsf/gocode', {'rtp': 'vim/'}
 Plugin 'Valloric/YouCompleteMe'
"Plugin 'Valloric/YouCompleteMe' {'do', './install.py'}
Bundle 'dgryski/vim-godef'
Bundle 'majutsushi/tagbar'
Plugin 'MarcWeber/vim-addon-mw-utils'
Plugin 'dzhou121/gonvim-fuzzy'     " Vundle
Plugin 'tomtom/tlib_vim'
Plugin 'garbas/vim-snipmate'
Plugin 'honza/vim-snippets'

call vundle#end()            " required
filetype plugin indent on    " required

set cursorline
set backspace=2
set autochdir
set ignorecase smartcase
set magic
set smartindent
set showmatch
set cindent
set autoindent
set shiftwidth=2
set confirm
set hlsearch
set incsearch
set gdefault
set wildmenu
set completeopt=preview,menu
set clipboard+=unnamed
set mouse=a
set selection=exclusive
set selectmode=mouse,key
set encoding=utf-8
syntax on
set nowritebackup nobackup
set tabstop=4
set nu!
set modelines=0 
set nu
execute pathogen#infect()
:nnoremap <CR> G
map <F2> :NERDTreeToggle<CR>

nmap <F8> :TagbarToggle<CR>
let g:tagbar_type_go = {
    \ 'ctagstype' : 'go',
    \ 'kinds'     : [
        \ 'p:package',
        \ 'i:imports:1',
        \ 'c:constants',
        \ 'v:variables',
        \ 't:types',
        \ 'n:interfaces',
        \ 'w:fields',
        \ 'e:embedded',
        \ 'm:methods',
        \ 'r:constructor',
        \ 'f:functions'
    \ ],
    \ 'sro' : '.',
    \ 'kind2scope' : {
        \ 't' : 'ctype',
        \ 'n' : 'ntype'
    \ },
    \ 'scope2kind' : {
        \ 'ctype' : 't',
        \ 'ntype' : 'n'
    \ },
    \ 'ctagsbin'  : 'gotags',
    \ 'ctagsargs' : '-sort -silent'
\ }
syntax enable
filetype plugin on
set number
colorscheme molokai
let g:go_disable_autoinstall = 0
