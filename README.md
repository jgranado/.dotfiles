first, install [janus](https://github.com/carlhuda/janus)

and add vim-powerline

  cd ~/.janus
  git clone git://github.com/Lokaltog/vim-powerline.git


then install tmux:

    brew install tmux

then:

    cd ~
    git clone git@github.com:tapster/.dotfiles.git
    ln -s .dotfiles/.tmux.conf .tmux.conf
    ln -s .dotfiles/.vimrc.after .vimrc.after
    ln -s .dotfiles/.vimrc.before .vimrc.before
    ln -s .dotfiles/.gvimrc.local .gvimrc.local
    ln -s .dotfiles/.zshrc .zshrc
    ln -s .dotfiles/.gitconfig .gitconfig

then
    Download and install a patched font from https://github.com/Lokaltog/powerline-fonts
    ln -s .dotfiles/.janus .janus
    hub clone Lokaltog/powerline ~/.janus/powerline
    echo 'set rtp+=~/.janus/powerline/powerline/bindings/vim` >> ~/.vimrc.before
    echo 'set guifont=Inconsolata-dz\ for\ Powerline:h12'  >> ~/.vimrc.before

