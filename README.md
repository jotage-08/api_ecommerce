## API E-Commerce
Este projeto é uma API de E-Commerce simples desenvolvida com Python e Flask, utilizando SQLite como banco de dados. A API é projetada para gerenciar produtos e realizar operações básicas de um sistema de e-commerce.

## Tecnologias Utilizadas

Python

Flask

SQLite

AWS Elastic Beanstalk

Swagger (para documentação)

Postman (para testes de API)

## Como Executar Localmente

Siga as etapas abaixo utilizando o terminal PowerShell. Certifique-se de que o Python 3.7 ou superior está instalado no seu sistema.

Clone o repositório no PowerShell:

git clone https://github.com/jotage-08/api_ecommerce.git

Entre no diretório do projeto:

cd api_ecommerce

Crie um ambiente virtual para isolar as dependências do projeto:

python -m venv venv


No Windows (PowerShell):

.\venv\Scripts\Activate

No Linux/Mac:

source venv/bin/activate

Você saberá que o ambiente foi ativado ao ver (venv) antes do caminho no terminal.

Instale as dependências listadas no arquivo requirements.txt:

pip install -r requirements.txt

Inicie o servidor da API executando:

python application.py
O servidor será iniciado, e o terminal mostrará algo como:

Running on http://127.0.0.1:5000/.
Pronto! Sua API E-Commerce está rodando localmente.

## Estrutura do Projeto

A estrutura do projeto é a seguinte:

```
E-Commerce/
├── application.py      # Código principal da API
├── requirements.txt    # Dependências
├── swagger.yaml        # Documentação OpenAPI
├── .gitignore          # Arquivos ignorados pelo Git
└── instance/
    └── ecommerce.db    # Banco de dados SQLite
```

## Como Fazer o Deploy na AWS Elastic Beanstalk

Este projeto está configurado para deployment no AWS Elastic Beanstalk. Atualmente, o serviço está desativado para evitar custos.

Se desejar ativá-lo, siga as etapas abaixo:

Instale a CLI do Elastic Beanstalk, caso ainda não tenha:

pip install awsebcli --upgrade

Inicialize o Elastic Beanstalk no projeto (se ainda não fez):

eb init
Faça o deploy manualmente:

eb deploy
Para monitorar o status do ambiente:

eb status
Atenção: Certifique-se de revisar os custos envolvidos antes de ativar o serviço.

## Variáveis de Ambiente

Se sua aplicação precisar de variáveis de ambiente, você pode criar um arquivo .env com o conteúdo necessário. Por exemplo:

SECRET_KEY=sua_chave_secreta
DATABASE_URL=sqlite:///instance/ecommerce.db

## Contribuição

Contribuições são bem-vindas! Se você quiser ajudar a melhorar o projeto, abra uma issue ou envie um pull request.
