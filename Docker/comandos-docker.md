# Comandos Docker

| Categoria | Comando | Descrição |
| --- | --- | --- |
| Start | `sudo systemctl start docker` | Inicia o docker na maquina caso não estiver iniciada |
| ▶️ Executar | `docker run <imagem>` | Baixa a imagem (se necessário) e executa um container |
| ▶️ Executar | `docker run --name mycontainer hello-world` | Cria e executa um container com nome personalizado |
| ▶️ Executar | `docker run --rm nginx` | Executa o container e remove automaticamente ao finalizar |
| 📋 Listar | `docker ps` | Lista apenas os containers em execução |
| 📋 Listar | `docker ps -a` | Lista todos os containers, inclusive os parados |
| 🛑 Controle | `docker stop <container>` | Para a execução de um container |
| 🛑 Controle | `docker start <container>` | Inicia um container parado |
| 🗑️ Remover | `docker rm <container>` | Remove um container parado |
| 🗑️ Remover | `docker rm -f <container>` | Remove o container mesmo que esteja em execução |
| 🗑️ Remover | `docker rm $(docker ps -a -q)`  | Remove todos os containers existente pois ele usa subcomando para trazer todos os containers |
| ⚙️ Execução | `docker exec <container> <comando>` | Executa um comando dentro do container |
| ⚙️ Execução | `docker exec <container> ls` | Executa o comando `ls` dentro do container |
| ⚙️ Execução | `docker exec -it <container> bash` | Acessa o terminal interativo (`bash`) do container |
| ❓ Ajuda | `docker run --help` | Exibe os parâmetros disponíveis do `docker run` |
| ❓ Ajuda | `docker run --help | grep name` | Filtra a ajuda buscando linhas que contenham `name` |