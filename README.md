# API de Consulta de Livros

## 1. Objetivo da API

Esta API foi desenvolvida utilizando Python e Flask com o objetivo de disponibilizar informações sobre livros em formato JSON.

A aplicação permite consultar uma lista de três livros, apresentando seus respectivos identificadores, títulos, autores e anos de publicação.

## 2. Tecnologias utilizadas

- Python
- Flask

## 3. Instalação das dependências

Primeiro, clone o repositório:

```bash
git clone https://github.com/gabrielfagnas/api-livros-flask.git
```

Entre na pasta do projeto:

```bash
cd api-livros-flask
```

Crie um ambiente virtual:

```bash
python -m venv venv
```

Ative o ambiente virtual no Windows:

```bash
venv\Scripts\activate
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

## 4. Como executar a aplicação

Após instalar as dependências, execute o seguinte comando:

```bash
python app.py
```

A aplicação será iniciada localmente no endereço:

```text
http://127.0.0.1:5000
```

## 5. Rota disponibilizada

A API disponibiliza a seguinte rota:

**GET /livros**

Endereço completo:

```text
http://127.0.0.1:5000/livros
```

Essa rota retorna uma lista de livros em formato JSON, contendo:

- ID do livro;
- Título;
- Autor;
- Ano de publicação.

## 6. Exemplo de resposta JSON

```json
{
  "livros": [
    {
      "id": 1,
      "titulo": "Dom Casmurro",
      "autor": "Machado de Assis",
      "ano": 1899
    },
    {
      "id": 2,
      "titulo": "O Cortiço",
      "autor": "Aluísio Azevedo",
      "ano": 1890
    },
    {
      "id": 3,
      "titulo": "A Hora da Estrela",
      "autor": "Clarice Lispector",
      "ano": 1977
    }
  ]
}
```
