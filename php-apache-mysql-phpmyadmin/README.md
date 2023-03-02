# PHP + Apache + MySQL + PHPMyAdmin

Ambiente contendo as 4 ferramentas do título.

## Pré Requisitos

Antes de começar, certifique-se de que você tem:

- Docker (_Docker version 23.0.1, build a5ee5b1_ ou superior)
- Docker Compose (_Docker Compose version v2.11.2_ ou superior)

## Como executar?

1. Navegue até a pasta raiz destes arquivos.
2. Copie o arquivo `./env/docker/.env.dist` para `./env/docker/.env`. No novo arquivo, `./env/docker/.env`, crie as
variáveis de ambiente que desejar. Por exemplo, nela está a variável que vai definir a senha de usuário ROOT no MySQL.
3. Execute o seguinte comando no terminal:

```bash
docker-compose up
```

O código da aplicação PHP deve ficar na pasta `./app`.

Depois disso, as aplicações estarão disponíveis nos seguintes endereços:

- `http://0.0.0.0:8000`: Apache + PHP
- `http://0.0.0.0:8080`: PHPMyAdmin

## Como Interromper?

1. Navegue até a pasta raiz destes arquivos.
2. Execute o seguinte comando no terminal:

```bash
docker-compose down
```
