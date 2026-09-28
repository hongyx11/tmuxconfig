# Tmux configuration

Canonical Oh My Tmux customizations, moved from `hongyx11/RemoteCppConfiger`.
The configuration is preserved unchanged as `tmux.conf.local`.

Use `./configmgr clone tmuxconfig` to clone this repository into
`${XDG_CONFIG_HOME:-$HOME/.config}/tmux` on each server.

RemoteCppConfiger's `macconfig/install_tmux.sh` and
`ubuntu_install_scripts/install_tmux.sh` install Oh My Tmux and TPM, then link
`~/.tmux.conf.local` to this checkout if that path is absent. Existing files and
symlinks are preserved. Tmux must already be installed.

If you already have `~/.tmux.conf.local`, compare it with this repository's
`tmux.conf.local` and preserve any machine-specific changes before replacing it
with a symlink. The compatibility link lets Oh My Tmux load the configuration
while the Git checkout stays in the config directory. Pulling updates then
updates the linked configuration; reload inside tmux with prefix + r.
