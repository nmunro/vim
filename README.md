
# Vim
My Vim config

# Instructions


### Getting sources
Clone into .vim

    git clone https://github.com/nmunro/vim .vim
    
 ### Configuring Plugins (first pass)
Activate the vundle submodule

    cd .vim
    git submodule init
    git submodule update

Install the plugins as a first pass (YouCompleteMe will fail at this step)

    vim +PluginInstall +qall

Configure [YouCompleteMe](https://github.com/Valloric/YouCompleteMe), please ensure you've got the dependencies installed and you have the right compilers and runtimes on your operating system. It's fairly easy to get up and running, but there are extra configuration steps that MUST be followed.

    cd .vim/bundle/YouCompleteMe
    ./install --clang-completer --js-completer --java-completer
   
### Configuring Plugins (second pass)

Install the plugins as was done so previously.

    vim +PluginInstall +qall
    
### Done
Happy Editing!
