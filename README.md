﻿# E-Commerce API

Este projeto é uma API para um sistema de E-Commerce desenvolvida em Python com Flask.

## Tecnologias Utilizadas
- **Python**
- **Flask**
- **SQLite**
- **AWS Elastic Beanstalk**
- **Swagger para documentação**

## Como Executar Localmente
1. Clone o repositório:
   \\\sh
   git clone https://github.com/jotage-08/api_ecommerce.git
   cd api_ecommerce
   \\\
2. Crie e ative um ambiente virtual:
   \\\sh
   python -m venv venv
   source venv/bin/activate  # No Windows use: venv\\Scripts\\activate
   \\\
3. Instale as dependências:
   \\\sh
   pip install -r requirements.txt
   \\\
4. Execute a aplicação:
   \\\sh
   python application.py
   \\\

## Estrutura do Projeto
\\\
E-Commerce/
├── application.py      # Código principal da API
├── requirements.txt     # Dependências
├── swagger.yaml         # Documentação OpenAPI
├── .gitignore           # Arquivos ignorados pelo Git
└── instance/
    └── ecomerce.db      # Banco de dados SQLite (não deve ser commitado)

\\\

## Deploy na AWS
Este projeto foi configurado para deploy no AWS Elastic Beanstalk, mas atualmente está fora do ar para evitar custos. Caso queira ativar o deploy, ajuste o arquivo .elasticbeanstalk/config.yml conforme necessário e esteja atento aos custos envolvidos.

## Contribuição
Sinta-se à vontade para abrir issues e pull requests!
