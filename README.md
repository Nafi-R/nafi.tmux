* HOW TO INSTALL


1. Clone the repository:
    ```bash
    git clone https://github.com/Nafi-R/nafi.tmux.git ~/.config/tmux
    ```

2. Source the configuration:
    ```bash
    tmux source-file ~/.config/tmux/tmux.conf
    ```
3. Restart tmux:
    ```bash
    tmux kill-server
    ```
4. Add tmux-sessionizer to your PATH and add CTRL+F to start tmux-sessionizer:
    ```bash
    echo 'export PATH="$PATH:$HOME/.config/tmux/tmux-sessionizer"' >> ~/.bashrc
    echo 'bind '"\C-f":"tmux-sessionizer\n"'' >> ~/.bashrc 
    source ~/.bashrc
    ```

5. Give execute permission to the tmux-sessionizer script:
    ```bash
    chmod +x ~/.config/tmux/tmux-sessionizer
    ```
6. Install the required dependencies:
    ```bash
    sudo apt install fzf ripgrep fd bat exa
    ```

