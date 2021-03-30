# new-install

## All the stuff needed for a new computer

### Homebrew

- Install Homebrew `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  `

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


### IDE

- Download from https://www.jetbrains.com/idea/download/#section=mac
- Import the settings Drive

### Command Line

- Download from https://iterm2.com/
- Install


### Node

### JQ

- Install with `brew install jq`


### Postman
