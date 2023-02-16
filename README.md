## Introduction

This repository serves as my way to help me setup and maintain my Mac. It takes the effort out of installing everything manually. Everything needed to install my preferred setup of macOS is detailed in this readme. Feel free to explore, learn and copy parts for your own dotfiles. Enjoy!

### Getting Started

1. Clone this repo to `~/dotfiles` with:

    ```zsh
    git clone --recursive git@github.com:highestblue/dotfiles.git ~/dotfiles
    ```

2. Make sure you have `curl` and `zsh` installed

3. Run the installation with:

    ```zsh
    ~/dotfiles/install
    ```
4. (Optional: Mac only) Install Homebrew & Mac apps specified in the [`Brewfile`](./Brewfile) with:

    ```zsh
    ~/dotfiles/mac-setup.sh
    ```

4. Restart your computer to finalize the process

### VSCode Dev-Container Setup

1. Open up your Settings JSON in VSCode by using the command pallete and typing "settings json" and add the following:

    ```zsh
    # Replace "highestblue" with your Github username if forking this repo
    "dotfiles.repository": "highestblue/dotfiles", 
    "dotfiles.installCommand": "~/dotfiles/install",
    "terminal.integrated.defaultProfile.linux": "zsh"
    ```

2. Start up your dev-container and you should see the same ZSH configuration & plugins that you have locally inside the container terminal. _If that doesn't work, try restarting VSCode and restarting the dev-container._

Your Mac is now ready to use!


