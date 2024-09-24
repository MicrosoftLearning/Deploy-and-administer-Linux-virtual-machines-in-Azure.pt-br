---
demo:
  title: 'Demonstração 02: Monitorar uma máquina virtual do Linux no Azure'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demonstração 02: Monitorar uma máquina virtual do Linux no Azure

## Tarefas de credenciais

+ Criar uma máquina virtual (Modelo de início rápido).
+ Configure os Insights da VM.
+ Criar um alerta.  
+ Identifique problemas de desempenho. 
+ Redimensione uma máquina virtual. 

## Requisitos de recursos

+ Máquina virtual do Azure (criar usando um modelo personalizado)

## Slides de referência 

+ Modelos do Azure Resource Manager
+ Principais recursos do Azure Monitor
+ Componentes do Azure Monitor
+ Métricas e logs

  
## Etapas de referência

Etapas detalhadas são fornecidas nesses links.

+ [Implantar uma VM simples do Ubuntu Linux](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-template)
+ [Habilitar os insights de VM para o agente do Azure Monitor](https://learn.microsoft.com/azure/azure-monitor/vm/vminsights-enable-portal#enable-vm-insights-for-azure-monitor-agent) 
+ [Tutorial: Criar um alerta de métrica para um recurso do Azure](https://learn.microsoft.com/azure/azure-monitor/alerts/alerts-create-metric-alert-rule)


## Slides de referência (opcional)

Use estes slides para contexto adicional.



## Pontos de discussão

1. Use **Implantar um modelo personalizado** para um computador Ubuntu Linux simples. É assim que os alunos criarão a VM no exercício. Discuta o uso de modelos. 

1. Habilitar Insights da VM. Revise como usar uma regra de coleta de dados e como selecionar um workspace do Log Analytics. 

1. Crie um alerta baseado em métricas. Por exemplo, crie uma nova regra de alerta com base no uso percentual da CPU.

1. Discuta o uso de grupos de ações e como atribuir um grupo de ações ao alerta. 

1. Revise como monitorar um alerta quando ele é acionado.

1. Feche com como exportar o modelo de recurso. 
