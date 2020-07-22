## O que é Docker?

Docker é uma interface amigável para interagir com a 
tecnologia LXC, além de ter uma estrutura de serviços
de internet, tornando a interação com container facili
tado.

- Criado pela Google
- Feito com linguagem Go
- Compartilha Kernel com o Host

## O que são Containers?

- Segregação de processos no mesmo Kernel (isolamento)
- Sistem de arquivos criado a partir de uma imagem
- Encapsula binários e libs necessárias para um app
- Algo como chroot(Inicia um processo em uma pasta específica) e uma VM

## O que são Imagens?

- Modelo de sistema de arquivos para criar um container(processo)

- São criadas a partir de um processo build (documento descritor, Dockerfile)

- Pode ser criado com um commit, acessando um container e modificando, a partir
de então criar uma nova imagem com essas alterações. (má prática)

- São compostas por uma ou mais camadas (layers), cada comando no Dockerfile é um

- Todas as layers que montam a imagem são somente leitura

- A junção de todas as camadas formam a imagem

- Apenas a última camada (layer) pode ser alterada

## Imagem vs Containers

- Relação de OOP, imagem docker como modelo(classe) e instanciar
o objeto seria o container
