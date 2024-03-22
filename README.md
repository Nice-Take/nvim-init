### Personalized NVIM setup
# Originally based on kickstart


### RASPBERRY PI INSTALL REQUIRES BUILDING BIN ###
git clone https://github.com/neovim/neovim

cd neovim

make CMAKE_EXTRA_FLAGS="-DCMAKE_INSTALL_PREFIX=$HOME/neovim"

get checkout stable

sudo make install
