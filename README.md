## All the stuff needed for a new computer

### Homebrew

- Install Homebrew `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`


### Git
- Install with `brew install git`
- Set up email in Git: `git config --global user.email "email@example.com"`
- Set up name in Git: `git config --global user.name "Mona Lisa"`
- Set up SSH. Doc `https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh`
- Create new SSH key `ssh-keygen -t ed25519 -C "your_email@example.com"`
- Start the agent in the background `eval "$(ssh-agent -s)"`
- Modify ssh.config `touch ~/.ssh/config` with
```
Host *
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_ed25519
```
- Add SSH key to agent `ssh-add -K ~/.ssh/id_ed25519`
- Copy key to GH account `pbcopy < ~/.ssh/id_ed25519.pub`


### Node

- Install nvm: `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash`


### Command Line

- Download from https://iterm2.com/
- Install Oh My ZSH `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
- Update `omz update`
- Create `touch ~/.profile`
- Copy profile
- Copy and replace .zshrc
- Install fonts `git clone https://github.com/powerline/fonts.git && cd fonts && ./install.sh`
- Change fonts on Iterm


### JQ

- Install with `brew install jq`


### IDE

- Download from https://www.jetbrains.com/idea/download/#section=mac
- Import the settings Drive

### Postman

- Download from https://www.postman.com/downloads/
