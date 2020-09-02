# Laboratório de Banco de Dados

Repositório criado com o propósito de reunir alguns dos principais bancos de dados e suas ferramentas de gerenciamento para os alunos da UFMS

## Instalação do Docker

```shell
curl -fsSL https://get.docker.com | sh
```

Por motivos de praticidade considere adicionar o usuário ao grupo "docker".

```shell
   usermod -aG docker $your_user
```

## Instalação do Docker-compose

Execute este comando para baixar a versão estável atual do Docker Compose:

```shell
   curl -L "https://github.com/docker/compose/releases/download/1.24.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

Aplique permissões executáveis ​​ao binário:

```shell
   chmod +x /usr/local/bin/docker-compose
```

Nota: Se o comando docker-compose falhar após a instalação, verifique a path. Você também pode criar um link simbólico para /usr/bin ou qualquer outro diretório em seu caminho

```shell
   ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```

## Remover os containers, volumes e network

```shell
   docker-compose down
```
