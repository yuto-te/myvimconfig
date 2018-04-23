### dein.vim(package manager)のインストール

```
cd ~/
curl https://raw.githubusercontent.com/Shougo/dein.vim/master/bin/installer.sh > installer.sh
mkdir ~/.cache/dein
sh ./installer.sh ~/.cache/dein
```

### vim/.vimrcとvim/dein.tomlのシンボリックリンクを$HOME/に追加する．
```
ln -sf vim/.vimrc ~/.vimrc
ln -sf vim/dein.toml ~/dein.toml
```

pluginを追加するときはdein.tomlに
```
[[plugin]]
repo = "repository/path" e.g.'Shougo/dein.vim'
```
を追加して，.vimrcに必要なものを追記する．
