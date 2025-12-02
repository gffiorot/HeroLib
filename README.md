# HeroTeams1103: API de Cadastro de hérois e times de heróis com Lib Modular

Este projeto demonstra a arquitetura **MVC com Repository** aplicada ao FastAPI, separando a lógica de **dados/serviço** (encapsulada na biblioteca `HeroTeams1103`) da lógica de **interface web** (Controller/Router na pasta `API`).

-----

## Requisitos & Configuração

### 1\. Stack & Requisitos

| Componente | Função |
| :--- | :--- |
| **Python** | 3.10+ |
| **`HeroTeams1103`** | Biblioteca de Serviço e Repositório Genéricos |

### 2\. Estrutura do Repositório

Seu projeto principal de execução (`API`) utiliza os componentes da biblioteca instalada.

```
.
├─ API/               # PASTA PRINCIPAL DE EXECUÇÃO
│  ├─ controllers/    
│  │   └─ (hero, generic e team)
│  ├─ main.py         # Codigo principal          
├─ HeroTeams1103/    
│  └─ (model, service, repository e util)
├─ README.md
├─ requirements.txt
├─ setup.py
└─ .gitignore
```

### 3\. Execução e Instalação

Tenha certeza que os requisitos estejam baixados.

1.  Crie o ambiente e instale as dependências:


```bash
python -m venv .venv

.venv\Scripts\Activate     # Linux/macOS: #source .env/bin/activate

# Instale a Lib e suas dependências
pip install HeroTeams1103
```

2.  Rode a aplicação (o Uvicorn aponta para `API/main.py`):

<!-- end list -->

```bash
# Uvicorn roda o módulo main dentro da pasta 'app'
uvicorn API.main:app --reload
```

  * A API estará acessível em: `http://127.0.0.1:8000`

-----

## Endpoints (Pessoas & Endereços)

  * **Documentação:** `http://127.0.0.1:8000/docs`