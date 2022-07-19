 # Desafio Backend

## Jogos disponíveis:
- Deve consumir de uma API e listar os jogos disponíveis
- Formato da API:
```
{
    "id": 3161272,
    "titulo": "São Paulo x Flamengo",
    "campeonato": "Brasileirão",
    "data": "2022-08-22",
    "opcoes": [
        { "1": 2.5 },
        { "x": 3.1 },
        { "2": 1.5 }
    ],
    "limites": [
        { "1": 150 },
        { "x": 500 },
        { "2": 750 }
    ]
}

```

- Formato a ser listado:
```
{
    "id": 3161272,
    "titulo": "São Paulo x Flamengo",
    "campeonato": "Brasileirão",
    "data": "2022-08-22",
    "opcoes": [
        { "casa": 2.5 },
        { "empate": 3.1 },
        { "fora": 1.5 }
    ]
}

```

- Deve ser possível consultar todos os eventos ou filtrar pelos campos: `id`, `campeonato` e `data`


## Venda:
- Durante a venda, deve ser informado o CPF o ID do evento, a opção selecionada e o valor da aposta
- Deve consultar na API se o CPF informado é válido
- A venda só pode ser realizada até o dia anterior ao evento
- O valor dos ganhos deve ser o valor da aposta multiplicado pelo valor da opção (Ex: casa = valor da aposta * 2.5)
- O valor da aposta deve ser menor que o limite estabelecido na opção do evento

--- 
## Adicionais

### Testes
- Os testes da API devem ser simulados localmente, NÃO devem consumir a API.

### Infraestrutura
- O projeto deve estar executando no Heroku e disponibilizada rota para testes.