# Machine Setup

### Directory Setup
```console
mkdir ~/projects
```

### [OhMyZsh](https://ohmyz.sh/)

```console
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### [Git SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

```console
ssh-keygen -t ed25519 -C "your_email@example.com"
```

```console
eval "$(ssh-agent -s)"
```

```console
touch ~/.ssh/config
```

```console
open ~/.ssh/config
```

```
Host github.com
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_ed25519
```


```console
ssh-add ~/.ssh/id_ed25519
```

```console
open ~/.zshrc
```

### Brew
```console
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```console
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/jaredgreen/.zprofile
```

```console
eval "$(/opt/homebrew/bin/brew shellenv)"
```

```console
brew install cask
```

### VSCode
```console
brew install --cask visual-studio-code
```