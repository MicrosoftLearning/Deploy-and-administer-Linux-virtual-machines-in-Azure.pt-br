---
demo:
  title: 'Demonstração 03: Acessar o armazenamento para uma máquina virtual Linux do Azure'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demonstração 03: Acessar o armazenamento para uma máquina virtual Linux do Azure

## Tarefas de credenciais

+ Criar uma máquina virtual (CLI).
+ Adicione discos de dados e configure partições. 
+ Monte um compartilhamento de arquivos do Azure SMB em uma VM do Linux.
+ Atribua uma identidade gerenciada em uma VM do Linux. 
+ Atribua funções do Azure. 
+ Transfira dados de e para uma VM do Linux usando o AzCopy. 

## Requisitos de recursos

Esses recursos podem ser criados antes ou durante a demonstração. 
+ Grupo de recursos
+ Máquina virtual do Linux.
+ Conta de armazenamento com compartilhamento de arquivo e contêiner de blob.
+ Arquivos carregados para usar para teste.
+ Identidade Gerenciada. 

## Etapas de referência

Etapas detalhadas são fornecidas nesses links.

+ [Início Rápido: Criar uma máquina virtual Linux com a CLI do Azure no Azure](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-cli)
+ [Anexar um disco de dados a uma VM do Linux](https://learn.microsoft.com/azure/virtual-machines/linux/attach-disk-portal)
+ [Criar um compartilhamento de arquivo SMB](https://learn.microsoft.com/azure/storage/files/storage-how-to-create-file-share?tabs=azure-portal)
+ [Introdução ao AzCopy](https://learn.microsoft.com/azure/storage/common/storage-use-azcopy-v10)


## Slides de referência

Use estes slides para contexto adicional. 
+ Contas de armazenamento
+ Contêineres e arquivos de blob
+ Arquivos versus blobs
+ Identidades gerenciadas
+ Controle de acesso baseado em função

## Pontos de discussão

**Criar uma máquina virtual usando a CLI** – Referência nº 1

>Você pode usar uma vm existente, em vez de criar outra.

1. Acessar o Cloud Shell.

1. Crie uma máquina virtual com a CLI. Saliente que esta é a terceira maneira pela qual os alunos demonstraram criar vms.
   
**Adicionar um disco de dados a uma máquina virtual Linux** – Referência nº 2

1. Revise como usar o portal para adicionar um disco de dados a uma máquina virtual. Os alunos usarão a CLI no exercício.

1. Conecte-se à máquina virtual e use `lsblk` para listar os discos. Observe o tamanho do disco e se o disco não está montado.

1. Prepare o disco com `parted` e `partprobe`. Use o código no link de referência.

1. Monte o disco e use `df` para listar o ponto de montagem. 

**Acessar um compartilhamento de arquivo SMB da máquina virtual** – Referência nº 3 e instruções do laboratório do aluno

1. Localize a conta de armazenamento e discuta os compartilhamentos de arquivos.

1. Atribua uma identidade gerenciada a uma máquina virtual. A identidade deve ter acesso à conta de armazenamento.

1. Copie o script do portal para acessar o compartilhamento de arquivo de uma máquina virtual Linux.

1. Conecte-se à máquina virtual e crie um arquivo com o script. Você pode usar o editor vi.

1. Execute o script e monte o compartilhamento de arquivo. 

**Use AzCopy para copiar um arquivo de blob para a unidade de dados** – Referência nº 4 e as instruções do laboratório do aluno.

1. Adicione a função Colaborador de Dados do Blob de Armazenamento à máquina virtual. Revise outras funções de blob. 

1. Conecte-se à máquina virtual e instale o AzCopy. Revise outras ferramentas que podem ser usadas para transferir arquivos. 

1. Use AzCopy para transferir um arquivo do armazenamento de blobs para a unidade de dados. Você também pode transferir um arquivo de volta para o armazenamento de blobs.  
