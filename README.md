E-Commerce API
API para um sistema de E-Commerce, desenvolvida em Python com Flask.

## Tecnologias Utilizadas
Python

Flask

SQLite

AWS Elastic Beanstalk

Swagger (para documentação)

Postman (para testes de API)

## Como Executar Localmente
Siga as etapas abaixo utilizando o terminal PowerShell. Certifique-se de que o Python 3.7 ou superior está instalado no seu sistema.

Clone o repositóri no PowerShell, execute:


git clone https://github.com/jotage-08/api_ecommerce.git

Depois troque de disco:

cd api_ecommerce

Ainda no PowerShell, crie um ambiente virtual para isolar as dependências do projeto:

python -m venv venv

Ative o ambiente virtual com o seguinte comando:

.\venv\Scripts\Activate

Você saberá que o ambiente foi ativado ao ver (venv) antes do caminho no terminal.

Instale as dependências: Com o ambiente virtual ativo, instale as dependências listadas no arquivo requirements.txt:

pip install -r requirements.txt

Inicie o servidor da API executando:

python application.py

O servidor será iniciado, e o terminal mostrará algo como:

Running on http://127.0.0.1:5000/.

E pronto, está rodando sua API E-Commerce

Estrutura do Projeto:

E-Commerce/
├── application.py      # Código principal da API
├── requirements.txt     # Dependências
├── swagger.yaml         # Documentação OpenAPI
├── .gitignore           # Arquivos ignorados pelo Git
└── instance/
    └── ecomerce.db      # Banco de dados SQLite 
    
## Deploy na AWS

Este projeto está configurado para deployment no AWS Elastic Beanstalk. Atualmente, o serviço está desativado para evitar custos. Se desejar ativá-lo, edite o arquivo .elasticbeanstalk/config.yml conforme necessário e faça o deploy manualmente. Certifique-se de revisar os custos envolvidos antes de ativar o serviço.

## Contribuição

Contribuições são bem-vindas! Abra uma issue ou envie um pull request.
