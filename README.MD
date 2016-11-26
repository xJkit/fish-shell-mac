# Awesome Fish Shell

> High User Experience shell. Never come back to BASH.

### Installation

In Mac OS, please use [brew](https://github.com/Homebrew/brew) to install fish:

```shell
$ brew install fish
```

then you are done! You can switch to fish shell by typing ``fish`` whenever you want.

### Set fish as default shell

Of course __BASH__ is default by now. You can set __fish__ as your default to substitute __BASH__ completely.

1. Open __/etc/shells__ file to append ``/usr/local/bin/fish`` at bottom line. Make Mac OS know the path of the fish shell execution file.
2. Change the default shell. Type:

```shell
$ chsh -s /usr/local/bin/fish
```
then you are done.

### Set the package manager for fish

Like __brew__, install [oh-my-fish](https://github.com/oh-my-fish/oh-my-fish), the package manager for fish shell. Just type:

```shell
$ curl -L http://get.oh-my.fish | fish
```
you need __git__@1.9.1+ pre-installed to make this command work properly. You can check via ``git --version ``, or update the git by `` brew upgrade git ``. If your git is not installed by ``brew``, please remove the git folder and re-install again by ``brew``. Git is located at: ``which git``.

With ``omf``, you can install whatever you want to make fish better suite your workflow.

### Enhance fish shell
There are several enhancement utilities to make fish better, though fish is already excellent.

1. [powerline-shell](https://github.com/banga/powerline-shell)
  * ``powerline-shell`` is a beautiful and useful prompt style for your shell.
  * You can install with __git__, or use ``omf`` to install ``bobthefish``.

2. [bobthefish](https://github.com/oh-my-fish/theme-bobthefish)
  * powerline-style directly for fish, installed by ``omf``:
  ```shell
  $ omf install bobthefish
  ```

  * You need patched fonts: [powerline fonts](https://github.com/powerline/fonts) to make these work correctly. Follow the github repo instructions, clone it, and run ``./install.sh``. Remember to change the shell fonts of the terminal emulator ([iTerm2](https://www.iterm2.com/) is preferable :>) at the preference setting (hotkey: __``cmd+,``__).


3. [agnoster](https://github.com/oh-my-fish/theme-agnoster)
  * A fish theme optimized for people who use __Git__, __SVN__ or Fish Vi-mode.
  ```shell
  $ omf install agnoster
  ```
