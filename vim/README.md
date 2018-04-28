This repository was originally a separate .vim.

Since handling sub-sub-modules in git was a bit of a pain in the ass, I decided simply copy my vim repository contets to my .dotfiles repository

Based on: https://shapeshed.com/vim-packages/

# Handlings packages

## Add a package
```bash
cd $VIM_FOLDER  # usually .vim/
git submodule init
git submodule add https://github.com/vim-airline/vim-airline
git add .gitmodules vim/pack/plugins/start/vim-airline
git commit
```

## Update a package
```bash
git submodule update --remote --merge
git commit
```

## Remove a package
```bash
git submodule deinit $VIM_FOLDER/pack/plugins/start/vim-airline
git rm $VIM_FOLDER/pack/plugins/start/vim-airline
rm -Rf .git/modules/vim/pack/plugins/start/vim-airline
git commit
```
