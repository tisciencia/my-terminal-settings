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