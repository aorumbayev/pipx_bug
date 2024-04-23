dummy cli to reproduce ImpImported bug

# Steps to reproduce

1. Launch codespace
2. curl https://pyenv.run | bash -> add pyenv to .bashrc
3. pyenv install 3.12.2
4. pyenv global 3.12.2
5. pipx install . --force --python $(which python)
6. pipx-bug-cli -> observe failing error
