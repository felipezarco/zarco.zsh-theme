# zarco.zsh-theme

Install oh-my-zsh with (if not already installed):

```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Create the theme file with:

```shell
sudo touch ~/.oh-my-zsh/themes/zarco.zsh-theme
```

Edit the file `~/.oh-my-zsh/themes/zarco.zsh-theme` with the editor you prefer to include this:

```shell
PROMPT=$'%{$fg_bold[green]%}%D{%I:%M} %{$reset_color%}%{$fg_bold[green]%}%~%{$reset_color%}$(git_prompt_info) %{$fg_bold[green]%}%{$fg_bold[green]%}\\$%{$reset_color%} '

ZSH_THEME_GIT_PROMPT_PREFIX="%{$fg_bold[white]%}("
ZSH_THEME_GIT_PROMPT_SUFFIX=")%{$reset_color%}"
ZSH_THEME_GIT_PROMPT_DIRTY=" %{$fg_bold[red]%}*%{$fg_bold[green]%}"
ZSH_THEME_GIT_PROMPT_CLEAN=""
```

Set `ZSH_THEME="zarco"` by editing `~/.zshrc`

Finally, refresh your terminal theme with `source ~/.zshrc`
