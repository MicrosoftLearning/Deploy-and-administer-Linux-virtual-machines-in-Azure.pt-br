---
demo:
  title: 'Demonstração 01: Configurar uma máquina virtual do Azure Linux'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demonstração 01: Configurar uma máquina virtual do Azure Linux

## Tarefas de credenciais

Use esta demonstração para revisar estas tarefas de credencial:
+ Crie uma máquina virtual do Linux (portal).
+ Configure uma VM do Linux.
+ Conecte-se a uma VM do Linux com SSH.  
+ Atualize sistemas operacionais de VM do Linux.
+ Instale e execute uma dependência de carga de trabalho.

## Requisitos de recursos

Esse recurso pode ser criado antes ou durante a demonstração. 

+ Grupo de recursos. 

## Slides de referência (opcional)

+ Plano para máquinas virtuais
+ Distribuições Linux compatíveis
+ Dimensionamento de máquina virtual
+ Organização de recursos do Azure
+ Ferramentas de Administrador do Azure

## Etapas de referência

Etapas detalhadas são fornecidas nesses links.

+ [Provisionar uma máquina virtual Linux usando o portal do Azure](https://learn.microsoft.com/training/modules/provision-linux-virtual-machine-in-azure/2-provision-linux-virtual-machine-using-the-azure-portal)
+ [Início Rápido: Criar uma VM do Linux](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-portal?tabs=ubuntu)

## Pontos de discussão

**Criação e configuração da máquina virtual**

1. Use o portal para criar uma VM do Linux. Discuta como, em exercícios posteriores, os modelos CLI e de início rápido serão usados para criar VMs. 

1. Use o link do portal para revisar a seleção de **Imagens** do Linux.  Identifique a distribuição mais recente do Ubuntu.

1. Use o link do portal para revisar as seleções de **Tamanho**.  Discuta como você pode dimensionar as configurações de CPU e memória.

1. Discuta os efeitos do redimensionamento. O redimensionamento será feito em um laboratório posterior. 

1. Discuta as diferentes maneiras de se conectar a uma máquina virtual Linux (chave pública SSH e senha).
   
1. Discuta a importância das **regras da porta de entrada**. Especificamente, a porta 22 para SSH e a porta 80 para Nginx. 

1. Use a guia **Discos** para mostrar como um disco dados seria adicionado. A adição de um disco de dados será feita em um exercício posterior. 
 
1. Use a página **Avançado** para mostrar onde um arquivo cloud-init pode ser fornecido.

1. Além disso, os exercícios posteriores usam modelos e a CLI para instalar máquinas virtuais. 

**Acesse a máquina virtual e instale o Nginx**

1. Implante a máquina virtual. Discuta a fase de validação e como monitorar as notificações.

1. Abra uma janela do CMD e acesse a máquina virtual com SSH. Discuta o formato do comando SSH e o local do arquivo de chave. 

1. Instale o Nginx e certifique-se de que a página inicial seja exibida. 
