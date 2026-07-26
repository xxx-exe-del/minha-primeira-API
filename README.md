# minha-primeira-api

## Instalação

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Execução

```bash
python3 vulnerable_app.py
```

O servidor sobe em `http://0.0.0.0:5000`.

## Endpoints

| Método | Rota            | Descrição                                  |
|--------|-----------------|---------------------------------------------|
| GET    | `/health`       | Verifica se o serviço está no ar             |
| POST   | `/register`     | Cria um novo usuário                         |
| POST   | `/login`        | Autentica e inicia sessão                    |
| POST   | `/logout`       | Encerra a sessão                             |
| GET    | `/whoami`       | Retorna o usuário logado                     |
| GET    | `/user/search`  | Busca usuários por campo (`field`, `q`)      |
| GET    | `/ops/ping`     | Testa conectividade com um host (`host`)     |
| GET    | `/export`       | Exporta os registros do usuário logado       |
| GET    | `/report`       | Relatório de eventos por período (admin)     |
| GET    | `/download`     | Baixa um arquivo de `reports/` (`name`)      |