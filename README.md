# UV
Um pacote Python extremamente rápido e gerenciador de projetos, escrito em Rust.

**Em resumo:** É o Cargo do Rust!

---
# Instalação
Rode `curl -LsSf https://astral.sh/uv/install.sh | sh` no seu terminal Linux/WSL, será instalado duas ferramentas, UV e UVX.
Em resumo, UV gerencia o projeto e UVX executa(mesmo sem criar venv ou instalar as depedências).

# Comandos gerais
- Executar programa `uvx main.py`.
- Criar projeto no diretório atual: `uv init .` 
- Criar projeto em um novo diretório: `uv init diretorio` 
- Instalar pacote(global) `uv tool install flake8`
- Para roda o flake8 `uv run flake8 main.py`
- Para escolher a versão do python `uv python install 3.12`
- Para criar venv `uv veenv --python 3.12`
- UV executa qualquer comando pip `uv pip install -r requirements.txt`

# Pyproject.toml
Usando os comandos de init é gerado esse arquivo, em resumo, o pyproject.toml é um arquivo padrão em projetos Python que centraliza configurações de ferramentas, dependências e métodos de build, simplificando o gerenciamento do projeto.

Tendo essa aparência:
```
[project]
name = "uv-learn"
version = "0.1.0"
description = "Add your description here"
readme = "README.md"
requires-python = ">=3.12"
dependencies = []

```
### comandos
- Para adicionar dependência `uv add dynaconf`
...
