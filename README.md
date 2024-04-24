dummy cli to reproduce ImpImported bug

# Steps to reproduce

1. Launch codespace
2. curl https://pyenv.run | bash
3. Add pyenv (see last lines from output of 2.) pyenv to .bashrc
4. pyenv install 3.12.2
5. pyenv global 3.12.2
6. pipx install . --force --python $(which python)
7. pipx-bug-cli -> observe failing error
