環境ごとに必ずインストールしたい物だけを書く  
個別に必要なものやアドホックに入れたものは管理しない  

brew bundle cleanupで一気に整理できるようにするため

## Brewfileからインストールする
```zsh
brew bundle --file $HOME/.brewfile/Brewfile
```

## Brewfileに居ないアプリを削除
Brewfileに記載のないアプリケーションをリスト表示する
```zsh
brew bundle cleanup --file $HOME/.brewfile/Brewfile
```
Brewfileに記載のないアプリケーションをアンインストールする
```zsh
brew bundle cleanup --force --file $HOME/.brewfile/Brewfile
```

## アップデートがあるパッケージ一覧
```zsh
brew outdated
brew outdated --cask
mas outdated
```