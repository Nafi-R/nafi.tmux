* HOW TO INSTALL


1. Install the required dependencies:
    ```bash
    sudo apt install tmux fzf

1. Clone the repository:
    ```bash
    git clone https://github.com/Nafi-R/nafi.tmux.git ~/.config/tmux
    ```

1. Source the configuration:
    ```bash
    tmux source-file ~/.config/tmux/tmux.conf
    ```
1. Restart tmux:
    ```bash
    tmux kill-server
    ```

1. Add the following line to your `~/.bashrc`:
    ```bash
    PATH="$PATH:"$HOME/.config/tmux/tmux-sessionizer"
    bind "\C-f":"tmux-sessionizer\n"
    ```

1. Update your directories in `~/.config/tmux/directories.conf` and `~/.confing/tmux/single-directory.conf`:
    ```bash
    # Example directories.conf
    # Add your directories here
    ~/projects
    ~/documents
    ~/downloads
    ```

1. Give execute permission to the tmux-sessionizer script:
    ```bash
    chmod +x ~/.config/tmux/tmux-sessionizer
    ```

