# how config your MAC for Stackeo 🙂

* installing 
* setting
* testing

## installing
* installing brew

in terminal
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

```
brew update
```
* installing bash
```
brew install bash 
```
* python 3.6

select the installer macOs in the section of file

 https://www.python.org/downloads/release/python-368/

* node
also before install node is more recommended instal nvm
```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```
after this command 
```
nvm install 14
```
* vs code
```
brew cask install visual-studio-code
```
* pycharm

go to pycharm url
https://www.jetbrains.com/pycharm/download/#section=mac


## setting

* vs code
installing all extension needing to make a great work 😆

make a file called vscode-extension.txt or whatever you want

```
nano vscode-extension.txt
```
in this fille paste the following line
```
andys8.jest-snippets
apollographql.vscode-apollo
christian-kohler.npm-intellisense
christian-kohler.path-intellisense
dbaeumer.vscode-eslint
dsznajder.es7-react-js-snippets
eg2.vscode-npm-script
esbenp.prettier-vscode
firsttris.vscode-jest-runner
formulahendry.auto-close-tag
formulahendry.auto-rename-tag
fosshaas.fontsize-shortcuts
ginfuru.ginfuru-onedark-raincoat-theme
HookyQR.beautify
JCsoftIA.jcsoftia
johnpapa.vscode-cloak
mhutchie.git-graph
mikestead.dotenv
ms-azuretools.vscode-docker
MS-CEINTL.vscode-language-pack-es
ms-mssql.mssql
ms-python.anaconda-extension-pack
ms-python.python
ms-vscode-remote.remote-ssh
ms-vscode-remote.remote-ssh-edit
ms-vscode.azure-account
ms-vscode.vscode-typescript-next
ms-vsliveshare.vsliveshare
msjsdiag.debugger-for-chrome
msjsdiag.vscode-react-native
Nimda.deepdark-material
Nur.just-black
Orta.vscode-jest
patbenatar.advanced-new-file
PKief.material-icon-theme
redhat.vscode-yaml
ritwickdey.LiveServer
SmukkeKim.theme-setimonokai
streetsidesoftware.code-spell-checker
Zignd.html-css-class-completion


```
in the terminal run
```
while read line; do code --install-extension "$line";done < vscode-extensions.txt
```
* terminal

in this case i use bash
for edited your profile you need created a new file called 
.bash_profile inside write your custom setting

* stackeo-main

it's time to clone stackilab in your 
```
git clone git@github.com:Stackeo-io/stackilab-main.git
```
if you don't have setting your ssh key you need do the following steps

in terminal
```
ssh-keygen -t rsa
````
copy the public key 

```
pbcopy < ~/.ssh/id_rsa.pub
```
and 

* Once you have copied your public SSH key, login to your GitHub account and go to
* https://github.com/settings/profile
* On the left-hand side menu, you will see a link “SSH and GPG keys”
* Click on that link which will take you to a page where you can enter your public SSH key that you copied earlier.
* Click the button which says ‘New SSH key’
* Then enter a title name - can be anything, e.g. newMac
* Paste the public SSH key in the key textbox
* Click “Add SSH key”

testing clone the stackilab repo

## testing

* alfred

```
pipenv install --dev pipenv shell . ./.alfred_pipenv_shell
```

for install alfred you need 


* deploy Stackeo

```
./alfred_bash
```


* enjoy 🍀