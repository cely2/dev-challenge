## Desafio Python Engineer

Crie um serviço em python que recebe mensagens via RabbitMQ, trata os dados e salva em um banco de dados.
Exemplo de mensagem:
```json
{
  "make": "Ferrari",
  "pilots": [
    {
      "name": "Vettel",
      "races": [
        {
          "year": 2020,
          "location": "Interlagos",
          "position": 3,
          "pole_position": true
        }
      ]
    },
    {
      "name": "Leclerc",
      "races": [
        {
          "year": 2020,
          "location": "Interlagos",
          "position": 1,
          "pole_position": false
        }
      ]
    }
  ]
}
```

## Requisitos
- RabbitMQ
- Banco de dados: MongoDB, MySQL ou PostgreSQL
- Testes unitários
- Processamentos que devem constar em banco:
    - Total de vitórias por ano
    - Total de poles por ano
    - Média de corridas que levaram ao pódio (até sexta colocação)
