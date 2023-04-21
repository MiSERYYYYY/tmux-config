# tmux-config

```
# Set the control character to Ctrl+Spacebar (instead of Ctrl+B)
# set -g prefix C-space
# unbind-key C-b
# bind-key C-space send-prefix

# Set mouse usage to on
set -g mouse on

# Set new panes to open in current directory
bind c new-window -c "#{pane_current_path}"
bind '"' split-window -c "#{pane_current_path}"
bind % split-window -h -c "#{pane_current_path}"


# Autoscroll when highlighting. e.g. copy pasting lots of text
set -g terminal-overrides 'xterm*:smcup@:rmcup@'

# history limit
set -g history-limit 50000

# prevents the pane from being auto renamed
set -g allow-rename off

# Start pane with 1 instead of 0
set -g base-index 1
setw -g pane-base-index 1

#
set -g renumber-windows on


```
# zsh autocomplete suggestion
https://github.com/zsh-users/zsh-autosuggestions
