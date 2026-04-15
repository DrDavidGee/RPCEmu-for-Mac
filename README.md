# RPCEmu-for-Mac

This repository currently contains only one file, **main_window.cpp**.

You should obtain RPCEmuBeta for Mac from https://github.com/riscosports/rpcemubeta.git

Then replace **rpcemubeta/src/qt5/main_window.cpp** with the mai_window.cpp found in this repository.

In other words, follow these instructions (based on https://www.riscosopen.org/forum/forums/5/topics/20192?limit=25&page=6#posts-163103):

1. Download main_window.cpp form this repository into your Downloads directory.
2. Install version 5 of Qt using Homebrew:

<code>
    brew install qt@5
    cd ~
    git clone https://github.com/riscosports/rpcemubeta.git
</code>

4. Replace the main_window.cpp found in the cloned rpcemubeta with the one in **Downloads**:

<code>
    rm ~/rpcemubeta/src/qt5/main_window.cpp
    cp ~/Downloads/main_window.cpp ~/rpcemubeta/src/qt5/main_window.cpp
</code>

5. Build the *interpreter* version of RPCEmu (it's the default):

<code>
cd ~/rpcemubeta/src/qt5
qmake rpcemu.pro
make
</code>

See also the later threds in the link given above.
