# setup-mac-dev

```shell
# Base
echo 'PATH="/usr/local/bin:$HOME/.local/bin/:$HOME/bin:$PATH"' >> $HOME/.zprofile

# ohmyzsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Homebrew
eval "$(/opt/homebrew/bin/brew shellenv)"

# Install Taskfile
sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b ~/.local/bin

# Composer auth.json
echo '{' >> $HOME/composer.auth.json
echo '    "github-oauth": {' >> $HOME/composer.auth.json
echo '        "github.com": "REPLACE_WITH_YOUR_TOKEN_HERE"' >> $HOME/composer.auth.json
echo '    }' >> $HOME/composer.auth.json
echo '}' >> $HOME/composer.auth.json
echo 'ALIAS composer-auth="ln -s $HOME/composer.auth.json auth.json"' >> $HOME/.zprofile
```
