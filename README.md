# mac setup

1. Install brave and import bookmarks
3. Install brew
4. Install iTerm2, create new profile and change the font (iTerm2 → Preferences → Profiles → Text)
5. Install go
6. Install python 3
7. Generate new SSH keys for github
8. Install intellij, python plugin and go plugin (GOROOT: /opt/homebrew/Cellar/go/1.18.1/libexec)
9. Dark mode: "System Preferences" and click "General"
10. Install oh-my-zsh
11. get plugins from github and edit ~/.zshrc:
```
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting

plugins=(
        fzf
        macos
        git
        golang
        docker
        kubectl
        zsh-autosuggestions
        zsh-syntax-highlighting
)

#   ---------------------------
#   Brew
#   ---------------------------
export HOMEBREW_NO_ANALYTICS=1

#   ---------------------------
#   Go
#   ---------------------------
export GOPATH="${HOME}/view/go"
export GO111MODULE=auto
```
