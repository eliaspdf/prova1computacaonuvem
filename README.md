# prova1computacaonuvem

# Prova 1 de Computação em Nuvem

Nome: Elias Pina de Faria
RA: d3394422fb7587039be4

## O que fiz

Executei uma página web em um contêiner Docker chamada loja.
Usei a imagem nginx:alpine e a porta 8081 do ambiente.

##Verificação do contêiner

docker ps
CONTAINER ID   IMAGE          COMMAND                  CREATED              STATUS              PORTS                                     NAMES
45d65b362b42   nginx:alpine   "/docker-entrypoint.…"   About a minute ago   Up About a minute   0.0.0.0:8081->80/tcp, [::]:8081->80/tcp   loja

##Teste da página 

curl http://localhost:8081
<!DOCTYPE html>
> <html lang="pt-BR">
> <head>
>  <meta charset="UTF-8">
>  <title>Loja</title>
</head>
<body>
 <h1>Loja no ar</h1>
</body>
</html>

##Explicação

a imagem é um modelo, e o contêiner é a instaância executada a partir dela.e o mapeamento 8081:80 serviu para ligar a porta do ambiente à porta do contêiner.
