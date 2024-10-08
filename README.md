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
 source ~/.nvm/nvm.sh
 nvm install v14.14.0
 ```
 ## Step 4: Install neovim 
 ```bash
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
chmod u+x nvim.appimage
./nvim.appimage

./nvim.appimage --appimage-extract
./squashfs-root/AppRun --version

# Optional: exposing nvim globally.
mv squashfs-root /
ln -s /squashfs-root/AppRun /usr/bin/nvim
nvim
 ```
 ## Step 5: cd ./config/nvim and clone git neovim
 ```bash
 cd 
 cd ~/.config/
 git clone https://github.com/phanben110/nvim.git
 ```
 ## Step 6: vim init.vim and :PlugInstall 
 ## Step 7: Install coc and coc-python
 nvim -c "PlugInstall" -c "qa"
* :CocInstall coc-json coc-tsserver
* :CocInstall coc-python
* Install coc python here https://github.com/neoclide/coc-python

 ## FULL BASH SHELL
 ```bash
sudo apt install curl
curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
source ~/.nvm/nvm.sh
nvm install v14.14.0
sudo add-apt-repository ppa:neovim-ppa/unstable
sudo apt-get update
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
chmod u+x nvim.appimage
./nvim.appimage

./nvim.appimage --appimage-extract
./squashfs-root/AppRun --version

# Optional: exposing nvim globally.
mv squashfs-root /
ln -s /squashfs-root/AppRun /usr/bin/nvim
nvim

cd
cd ~/.config/
git clone https://github.com/phanben110/nvim.git

nvim -c "PlugInstall" -c "qa"
nvim -c "CocInstall coc-json coc-tsserver" -c "qa"
nvim -c "CocInstall coc-python" -c "qa"
nvim -c "CocInstall coc-clangd" -c "qa"

echo "alias vi='nvim'" >> ~/.bashrc
echo "alias nv='nvim'" >> ~/.bashrc
sleep 2
source ~/.bashrc


echo "+++++++++++Install Neovim Sucessful++++++++"
 ```
