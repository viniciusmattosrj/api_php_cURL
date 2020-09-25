# Sobre o Projeto
Como consumir API no PHP com cURL.
- <a href="https://www.youtube.com/watch?v=tIterRjj8mk">API PHP cULR</a> - Celke


## Requerimentos

- Install <a href="https://docs.docker.com/install/">Docker</a>

- Install <a href="https://docs.docker.com/compose/install/">docker-compose</a>

- PHP >= 7.3

- Postgres >= 9.6 ou Mysql >= 5.7


## Instalação
Realizar o git clone do projeto base para o funcionamento da sua rede docker:
```bash
git@github.com:viniciusmattosrj/projetos.git
```

Para que o git não considere alterações de permissão como modificações a serem rastreadas, execute:
```
git config core.fileMode false
```

Agora suba o servidor:
```
docker-compose up -d
```

Navege até dentro da pasta projetos e realize o git clone do projeto
```bash
cd projetos && git@github.com:viniciusmattosrj/api-php-curl.git
```

Para que o git não considere alterações de permissão como modificações a serem rastreadas, execute:
```
git config core.fileMode false
```

Entre pelo terminal na pasta do projeto e rode:
```
cp ./docker-compose-example.php  ./docker-compose.php
```

Agora suba o servidor:
```
docker-compose up -d
```

Em outra aba do terminal se conecte no container do php e inicie um servidor built in do PHP
```
docker exec -it php bash
php -S 10.11.0.11:8008 -t .
```

No browser digite http://10.11.0.11:8008

## Contribuições
Caso identifique pontos
que possam ser aprimorados envie o seu PR. ;-)


## License
[MIT](https://choosealicense.com/licenses/mit/)