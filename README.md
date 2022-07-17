# Shell

This repo contains my custom configuration of the z-shell. It depends on `zsh` and `starship`. To configure it, all you need to do is clone this repository into the `.zsh/` folder and replace the `.zshrc` file with the `rc` file in this repo.

```bash
$ sudo dnf install zsh starship
$ git clone https://github.com/modzilla99/shell ~/.zsh
$ pushd ~/.zsh
$ git submodule update --init --recursive
$ popd
$ cp -f ~/.zsh/rc ~/.zshrc
```

## Adding missing completions

To add completions to zsh, you can easily add the appropriate files to the `$ZSH_HOME/completions/` directory.

for example:
```bash
$ kubectl completion zsh > $ZSH_HOME/completions/__kubectl
```
