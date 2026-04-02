# Portfolio - Desafio Docker Apache

Este projeto demonstra a execução de uma aplicação de portfólio de alta qualidade rodando em um servidor Apache provido via Docker Compose. O layout emprega padrões modernos de UI/UX como Glassmorphism, animações fluidas e design responsivo, sem utilizar frameworks externos - 100% Vanilla HTML/CSS/JS.

## Requisitos

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Git](https://git-scm.com/)

## Como Executar

1. Clone ou baixe este repositório.
2. Navegue até o diretório raiz do projeto onde encontra-se o arquivo `docker-compose.yml`.
3. Execute o comando para iniciar o contêiner em segundo plano:
   ```bash
   docker-compose up -d
   ```
4. Acesse a aplicação no seu navegador:
   [http://localhost:8085](http://localhost:8085)

## Como Subir para o seu GitHub

Para subir este projeto para o seu próprio repositório no GitHub para compor seu portfólio, siga os passos abaixo no terminal do diretório raiz:

```bash
git init
git add .
git commit -m "feat: implementa portfolio com apache dockerizado"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git
git push -u origin main
```

## Arquitetura

O projeto consiste de três partes fundamentais:
- Arquivo `docker-compose.yml` que provisiona e redireciona portas do container `httpd:latest`.
- O mapeamento de volume lógico que liga a pasta host `./html` à pasta hóspede `/usr/local/apache2/htdocs/`.
- Desenvolvimento Web frontend responsivo e esteticamente refinado.
