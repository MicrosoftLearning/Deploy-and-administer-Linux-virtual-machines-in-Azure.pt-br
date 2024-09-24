---
demo:
  title: 'Demonstração 04: Fazer backup de máquinas virtuais do Linux no Azure'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demonstração 04: Fazer backup de máquinas virtuais do Linux no Azure

## Tarefa de credenciais

+ Configurar o Backup do Azure 

## Requisitos de recursos

+ Máquina virtual do Linux

## Etapas de referência

Etapas detalhadas são fornecidas neste link.

+ [Início Rápido: Fazer backup de máquinas virtuais no portal](https://learn.microsoft.com/azure/backup/quick-backup-vm-portal)
+ [Início Rápido: Criar e implantar modelos do ARM usando o portal do Azure](https://learn.microsoft.com/azure/azure-resource-manager/templates/quickstart-create-templates-use-the-portal)

## Slides de referência

Use estes slides para contexto adicional.  

+ O que é o Backup do Azure?
+ Opções para proteger máquinas virtuais

## Pontos de discussão

1. Revise a importação de um modelo. Esta é a quarta maneira de criar uma vm em classe.
   
1. Discuta a necessidade de um cofre dos serviços de recuperação. O cofre deve estar na mesma região da fonte de dados. 

1. Revise como o backup da máquina virtual pode ser acessado e habilitado no portal. 

1. Discuta a diferença entre as políticas de backup Standard e Avançado. 

1. Use o menu suspenso **tipo de fonte de dados** para revisar os recursos que o Centro de Backup pode proteger.

1. Indique a política de backup padrão e que uma política de backup personalizada pode ser criada.

1. Discuta como uma única política de backup pode ser usada em muitas máquinas virtuais diferentes.

1. Revise as definições de configuração da política de backup (agendamento e retenção).

1. Revise como monitorar trabalhos de backup.

1. Revise como você pode restaurar máquinas virtuais (não na credencial). 
