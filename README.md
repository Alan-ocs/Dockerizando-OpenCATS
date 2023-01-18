# OpenCATS on Docker

Este repositório contém um arquivo Dockerfile para construir uma imagem Docker do [OpenCATS](https://github.com/opencats/OpenCATS) - um sistema de gerenciamento de candidaturas de código aberto. 

A imagem inclui o Ubuntu como base, as dependências necessárias para o OpenCATS, o Apache2 como servidor web, o MariaDB como banco de dados e o PHP como interpretador.

## Como usar

1. Clone este repositório

git clone https://github.com/seu-usuario/opencats-docker.git


2. Entre no diretório do repositório

cd opencats-docker

3. Construa a imagem


docker build -t opencats .


4. Inicie o container


docker run -p 80:80 opencats

Isso vai expor a porta 80 do container para a porta 80 do host, permitindo que você acesse o OpenCATS através do seu navegador usando o endereço IP do host ou o nome do host.

Observe que é necessário configurar o banco de dados e o arquivo de configuração do aplicativo antes de usar o OpenCATS. As instruções de instalação podem ser encontradas na [documentação do OpenCATS](https://github.com/opencats/OpenCATS/blob/master/docs/INSTALL.md)

