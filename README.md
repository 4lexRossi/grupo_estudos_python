# Pyenv
##### Windows
1. Instale o pyenv `pip install pyenv-win --target $HOME\.pyenv`
2. Adicione PYENV nas variáveis de ambiente `[System.Environment]::SetEnvironmentVariable('PYENV',$env:USERPROFILE + "\.pyenv\pyenv-win\","User")`
3. Adicione os binários do pyenv no path `[System.Environment]::SetEnvironmentVariable('path', $HOME + "\.pyenv\pyenv-win\bin;" + $HOME + "\.pyenv\pyenv-win\shims;" + $env:Path,"User")`

##### Linux
1. Instale o pyenv `curl https://pyenv.run | bash`
2. Adicione o seguinte no .bashrc:
    ```sh
    export PATH="$HOME/.pyenv/bin:$PATH"
    eval "$(pyenv init -)"
    eval "$(pyenv virtualenv-init -)"
    ```
3. Reinicie o shell `exec $SHELL`

Após seguir os passos acima, digite `pyenv --version` e verifique se a instalação foi feita corretamente.

#### Mais informações:
[Windows](https://pypi.org/project/pyenv-win/)  
[Linux](https://github.com/pyenv/pyenv-installer)  
[Projeto do Pyenv](https://github.com/pyenv/pyenv)

Para listar as versões do python `pyenv install -l` e para instalar `pyenv install <versao>`.

Erros podem ocorrer durante a instalação do pyenv ou do python, verifique a lista de [erros comuns](https://github.com/pyenv/pyenv/wiki/Common-build-problems).

#### Virtualenv
Criar ambiente virtual `pyenv virtualenv <versao_do_python> <nome_do_ambiente>`.
Listar ambientes virtuais `pyenv virtualenvs`.
Ativar ambiente virtual `pyenv activate <nome_do_ambiente>`.
Sair do ambiente virtual `pyenv deactivate`.

# Pycharm
[Instalação](https://www.jetbrains.com/help/pycharm/installation-guide.html)  
[Instalação em pt-BR](https://www.jetbrains.com/pt-br/pycharm/download/#section=linux)
