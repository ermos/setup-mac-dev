# setup-mac-dev

```
# ohmyzsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Homebrew
echo "PATH="/usr/local/bin:$PATH"" >> ~/.profile
eval "$(/opt/homebrew/bin/brew shellenv)"

# Jetbrains cli helper
echo "export IJ_LAUNCHER_DEBUG=true" >> ~/.profile
echo "export IDEA_LAUNCHER_DEBUG=true" >> ~/.profile
echo 'ALIAS webstorm="open -a ~/Applications/WebStorm.app/Contents/MacOS/webstorm"' >> ~/.profile
echo 'ALIAS phpstorm="open -a ~/Applications/PhpStorm.app/Contents/MacOS/phpstorm"' >> ~/.profile
echo 'ALIAS goland="open -a ~/Applications/GoLand.app/Contents/MacOS/goland"' >> ~/.profile
echo 'ALIAS aqua="open -a ~/Applications/Aqua.app/Contents/MacOS/aqua"' >> ~/.profile
```
