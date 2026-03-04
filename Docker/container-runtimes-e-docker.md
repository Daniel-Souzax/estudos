# Container Runtimes e Docker

- Criado em 2013 por uma empresa chamada dotCLoud (PaaS) para uso interno
- Docker Engine passou a ser Open Source
- Com a popularização da ferramenta, a dotCloud foi renomeada para Docker Inc.
- Docker CE / Engine é diferente do Docker Desktop (produto da Docker Inc.)
- Docker utiliza os recursos do Linux e outros componetes
    - Ferramenta 360: gerenciamento de containers, rede e disco, além da crianção e build de imagens
    - Trabalha no formato cliente-servidor e é um CLI (command line interface)
        - Daemon (dockerd) que faz o gerenciamento de todos os containers
        - Client que faz chamadas para o deamon
        - Daemon acaba se tornando um ponto único de falha (SPoF)
            - Root vs rootless