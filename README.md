# git

## git settings 

run `git config --global --edit`

add this settings

```
[user]
    email = tisciencia@gmail.com
    name = Tiago Sciencia
[core]
    editor = code --wait
[push]
    followTags = true
[alias]
    s = !git status -s
    c = !git add --all && git commit -m
    l = !git log --pretty=format:'%C(yellow)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
```


## instal zsh

run `brew install zsh`


## install oh my zsh

run `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`


## plugins do zsh

Para instalar plugins precisamos configurar o ZInit, ferramenta que facilita a instalação e remoção de plugins no Zsh.

`bash -c "$(curl --fail --show-error --silent --location https://raw.githubusercontent.com/zdharma-continuum/zinit/HEAD/scripts/install.sh)"`

Após essa instalação, vamos abrir o arquivo `~/.zshrc` novamente e abaixo da linha `### End of ZInit's installer chunk` que foi adicionada automaticamente no arquivo, adicionamos:

```
zinit light zdharma/fast-syntax-highlighting
zinit light zsh-users/zsh-autosuggestions
zinit light zsh-users/zsh-completions
```
