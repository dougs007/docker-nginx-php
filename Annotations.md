## Anotações do Projeto

  Criado uma aplicação PHP com servidor NGINX utilizando Docker. Foi usada a imagem do nginx e 
php em suas versões alpine.

## Informações técnicas utilizadas

  Linkado os serviços dentro do docker-compose.yml para utilizar dentro do arquivo de configurações do
nginx. Feito os volumes (espelhos) para tudo que for modificado da aplicação ser refletido dentro 
do container, como da aplicação (app) como do diretório docker (configurações)

## Comandos utilizados

Subir a aplicação.
> $  docker-compose up

Subir a aplicação em background.
> $  docker-compose up -d

Recriar a(s) imagem(s).
> $  docker-compose build

Executar um comando dentro do container chamado web.
> $  docker-compose run web cat etc/nginx/conf.d/default.conf
