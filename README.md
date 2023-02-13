# Mac setup

1. Install brew
2. Install brave and import bookmarks
3. Install bitwarden
4. Key-speed: System-Preferences → Keyboard → set to fast
5. Install iTerm2, create new profile and change the font (iTerm2 → Preferences → Profiles → Text), set Alt/Cmd + Right/Left Arrow (iTerm2 → Preferences → Profiles → Keys → Key Mappings → Presets... → Natural Text Editing)
6. Install gcloud
7. Install kubectl
8. `brew install go`
9. Install python 3
```
brew install python@3.10
brew unlink python@3.9
brew link --force python@3.10
python3 --version
```
10. [Generate new SSH keys for github](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
11. Set git username and email
```
git config --global user.name "username"
git config --global user.email "MY_NAME@example.com"
```
12. Install intellij, python plugin and go plugin (GOROOT: /opt/homebrew/Cellar/go/1.18.1/libexec)
13. Dark mode: "System Preferences" and click "General"
14. Container runtime [calima](https://github.com/abiosoft/colima/):
```
brew install docker
brew install colima
```
15. Install oh-my-zsh
16. get plugins from github and edit ~/.zshrc:
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
brew install fzf
brew install zsh-autosuggestions
```
```
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

# Apps
1. Bitwarden
2. Spotify
3. Slack
4. VSCode
5. iTerm2

# VSCode Shortcuts
1. Quick file open: Command + P 
2. Open terminal: Ctrl + `
3. Move line: Option + Up/Down arrow
4. Rename: F12
5. Select current line: Command + L
6. Duplicate line: Shift + Option + Down/Up
