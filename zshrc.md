# Path to your oh-my-zsh installation.
export ZSH=/Users/aya/.oh-my-zsh


# git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
# ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
# git icon broken fix https://github.com/spaceship-prompt/spaceship-prompt/issues/604 https://stackoverflow.com/questions/59128426/firacode-ligatures-not-working-in-iterm-2
ZSH_THEME="spaceship"

# git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
# git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
# git clone https://github.com/agkozak/zsh-z $ZSH_CUSTOM/plugins/zsh-z
plugins=(
  git
  zsh-autosuggestions
  zsh-syntax-highlighting
  zsh-z
)


# https://omyz.sh/
source $ZSH/oh-my-zsh.sh

#
# alias zshconfig="mate ~/.zshrc"
# alias ohmyzsh="mate ~/.oh-my-zsh"
  
# For Python
alias p3="python3"
export PATH="/usr/local/sbin:$PATH"

# For react-native
alias rn="react-native"

# For MySQL
alias mysql="sudo /usr/local/mysql/bin/mysql"
alias mysql-start="sudo /usr/local/mysql/support-files/mysql.server start"
alias mysql-stop="sudo /usr/local/mysql/support-files/mysql.server stop"
alias mysql-restart="sudo /usr/local/mysql/support-files/mysql.server restart"
alias mysql-login="sudo /usr/local/mysql/bin/mysql -u root -p"

# For Android SDK
export ANDROID_HOME=~/Library/Android/sdk
export PATH=${PATH}:${ANDROID_HOME}/tools
export PATH=${PATH}:${ANDROID_HOME}/platform-tools
export PATH=${PATH}:/Library/Java/JavaVirtualMachines/jdk1.8.0_101.jdk/Contents/Home

export PATH=${PATH}:${ANDROID_HOME}/ndk-bundle

export PATH=${PATH}:/Users/aya/Library/Android/flutter/bin
export PUB_HOSTED_URL=https://pub.flutter-io.cn
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

#deno
export DENO_INSTALL="/Users/aya/.deno"
export PATH="$DENO_INSTALL/bin:$PATH"

#Chrome
alias chrome="/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrom"
alias chrome-canary="/Applications/Google\ Chrome\ Canary.app/Contents/MacOS/Google\ Chrome\ Canary"
alias chromium="/Applications/Chromium.app/Contents/MacOS/Chromium"
export PATH="/usr/local/opt/curl/bin:$PATH"

#GCC
export LDFLAGS="-L/usr/local/opt/curl/lib"
export CPPFLAGS="-I/usr/local/opt/curl/include"

# rust
export PATH="$PATH":"$HOME/.pub-cache/bin"

