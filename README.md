# Personalized NVIM setup
### Originally based on kickstart


## Mac Install ###
mkdir -p ~/.config/nvim
nvim_config=~/config/nvim/inti.lua


## RASPBERRY PI INSTALL REQUIRES BUILDING BIN ###
git clone https://github.com/neovim/neovim

cd neovim

make CMAKE_EXTRA_FLAGS="-DCMAKE_INSTALL_PREFIX=$HOME/neovim"

git checkout stable

sudo make install

sudo mv ./bin/nvim /bin

## Add to PATH

nano ~/.bashrc

export PATH="$HOME/neovim/bin:$PATH"

source ~/.bashrc

