# Configurar o alembic
## Inicie o elembic
No terminal: python -m alembic init migrations

# Edite o arquivo alembic.ini na linha 89 e deixe assim:
sqlalchemy.url =
## Depois edite o arquivo migrations/env.py

# Rodar o alembic - criar uma migrations
python -m  alembic revision --autogenerate -m "Criar tabela usuarios"
## Aplique a migration
python -m alembic upgrade head