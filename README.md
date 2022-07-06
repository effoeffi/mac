# mac setup

1. Install brave and import bookmarks
3. Install brew
4. Key-speed: System-Preferences → Keyboard → set to fast
5. Install iTerm2, create new profile and change the font (iTerm2 → Preferences → Profiles → Text), set Alt/Cmd + Right/Left Arrow (iTerm2 → Preferences → Profiles → Keys → Key Mappings → Presets... → Natural Text Editing)
6. Install gcloud
7. Install kubectl
8. Install go
9. Install python 3
```
brew install python@3.10
brew unlink python@3.9
brew link --force python@3.10
python3 --version
```
7. Generate new SSH keys for github
8. Install intellij, python plugin and go plugin (GOROOT: /opt/homebrew/Cellar/go/1.18.1/libexec)
9. Dark mode: "System Preferences" and click "General"
11. container runtime [calima](https://github.com/abiosoft/colima/)
12. Install oh-my-zsh
13. get plugins from github and edit ~/.zshrc:
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

# apps
1. Bitwarden
2. Spotify
