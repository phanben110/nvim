# Install plugin neovim
## Step 1: Install curl
```bash
 sudo apt install curl
 
```
## Step 2: Install nvm 
```bash
 curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
```
## Step 3: Install node JS v14.14.0
```bash 
 nvm install v14.14.o
 ```
 ## Step 4: Install neovim 
 ```bash
sudo add-apt-repository ppa:neovim-ppa/unstable
sudo apt-get update
sudo apt-get install neovim
 ```
 ## Step 5: cd ./config/nvim and clone git neovim
 ```bash
 cd 
 cd .config/ 
 git clone https://github.com/phanben110/nvim.git
 ```
 ## Step 6: vim init.vim and :PlugInstall 
 ## Step 7: Install coc and coc-python
* :CocInstall coc-json coc-tsserver
* :CocInstall coc-python
* Install coc python here https://github.com/neoclide/coc-python
