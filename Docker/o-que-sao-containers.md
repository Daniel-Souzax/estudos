# O que são containers

Um container é uma unidade padronizada de software que empacota o código e todas as suas dependências para que um software seja executado de forma rápida e consistente em qualquer ambiente. 

### Principais características

- Imutabilidade
- Isolamento de processos e recursos computacionais
- Leves - É executado como um processo no sistema operacional
- Utilizam os recursos do Kernel de SO - Não possui a necessidade de instalar um novo SO
    - O container é “enganado” pensando que ele tem um SO próprio
    - A visibilidade dos processos é limitada aos processos gerados por ele
- Rápido de iniciar e de ser removido ou parado - Não há necessidade de “boot”
- Utilizam “imagens” (imutáveis) para serem executados - *Algo similar a um snapshot*

### Container vs Máquinas Virtuais

- Máquinas Virtuais (VMs):
    - Cada VM executa um sistema operacional completo, incluindo o kernel, e utiliza um hypervisor para gerenciar várias VMs no mesmo hardware. Isso resulta em maior consumo de recursos, maior tempo de inicialização e menor eficiência em termos de uso de memória e CPU
- Containers
    - Compartilham o kernel do sistema operacional do host, isolando apenas o aplicatrivo e suas dependências. Isso os torna significativamente mais leves, permitindo um uso mais eficiente de recursos e uma inicialização quase instantânea. Containers são ideais para cenários que exigem rápida escalabilidade e alta densidade de aplciativos em um único host.