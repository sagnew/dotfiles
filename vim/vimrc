"simple vimrc that I give to people just starting to use Vim."


"Turns on syntax highlighting"
syntax on


"Basic settings"
set nocompatible "Fixes old Vi bugs"
set backspace=indent,eol,start "Makes backspace work"
set history=500 "Sets undo history size"
set ruler "Sets up status bar"
set number "Turns on line numbering"
set tabstop=4 "Sets indent size of tabs"
set softtabstop=4 "Soft tabs"
set expandtab "Tabs suck. Spaces rule."
set shiftwidth=4 "Sets auto-indent size"
set laststatus=2 "Always keeps the status bar active"
set autoindent "Turns on auto-indenting"
set smartindent "Remembers previous indent when creating new lines"
set cursorline
set cursorcolumn
set t_Co=256 "Sets terminal to use 256 colors"

"Sets colorscheme to elflord"
colorscheme elflord


"Search settings"
set hlsearch "Highlights search terms"
set showmatch "Highlights matching parentheses"
set ignorecase "Ignores case when searching"
set smartcase "Unless you put some caps in your search term"


"Key mappings"
inoremap jj <Esc>`^
set pastetoggle=<F2>


"Window movement mappings"
nnoremap <c-h> <c-w>h
nnoremap <c-l> <c-w>l
nnoremap <c-j> <c-w>j
nnoremap <c-k> <c-w>k

"Filetype settings"
filetype plugin indent on "Turns on plugin/indentation support for specific filetypes"

"Allow crosshair cursor highlighting."
hi CursorLine   cterm=NONE ctermbg=235
hi CursorColumn cterm=NONE ctermbg=235
nnoremap <Leader>c :set cursorline! cursorcolumn!<CR>

au FileType make setlocal noexpandtab

"Gets rid of trailing whitespace"
autocmd BufWritePre * :%s/\s\+$//e


"Vundle stuff"
"
set nocompatible               " be iMproved
filetype off                   " required!

set rtp+=~/.vim/bundle/vundle/
call vundle#rc()

Bundle 'gmarik/vundle'
Bundle 'tpope/vim-fugitive'
Bundle 'kchmck/vim-coffee-script'

filetype plugin indent on
