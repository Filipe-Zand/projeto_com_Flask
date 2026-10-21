# Documentação: Instalação do uv e Python no VS Code
1. Abrir o terminal
Abrimos o VS Code para abrir o terminal PowerShell.
2. Instalar o uv
Executamos o comando para instalar o uv utilizando o Bypass, necessário para contornar restrições de execução de scripts do PowerShell.
powershell -ExecutionPolicy Bypass -c "irm https://astral.sh/uv/install.ps1 | iex"
3. Verificar a instalação do uv
uv -V
4. Instalar e verificar o Python 3.15
uv python install 3.15
uv python list
uv run -python 3.15 python -V
5. Criar e ativar o ambiente virtual
uv venv -python 3.15
.\.venv\Scripts\Activate.ps1
6. Verificar o Python
python --version
# Conclusão
Com esses comandos, instalamos o uv, configuramos o Python 3.15, criamos um ambiente virtual e instalamos as bibliotecas necessárias para desenvolver projetos Python no VSCode.
