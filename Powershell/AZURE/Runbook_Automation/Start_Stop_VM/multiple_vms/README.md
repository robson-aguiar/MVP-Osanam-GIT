# [Start-Stop] Runbook Azure Automaton - Múltiplas VM´s

Para que possamos rodar iniciar e parar múltiplas VM´s precisamos efetuar os seguintes passos:

1. Criar uma conta no Azure Automation
2. Criar um Runbook Powershell
3. Editar o Runbook Powershell e colar o script
4. Ao criar/rodar o script, devemos passar os seguintes parâmetros:
*    RESOURCEGROUPNAME
    <BR>Nome do Grupo de Recursos onde se encontram as VM´s
    <BR>

*    RESOURCENAME
     <BR>Neste campo você incluirá a relação de VM´s que será ligadas/desligadas.
     <BR>É necessário adicionar as mesmas no forma de array JSON, pois no Azure Automation entende array´s desta forma conforma exemplo abaixo:
     <BR>
     
     <code>['vm01','vm02','vm03']</code>

*    ACAO
    <BR>Insira opção de Iniciar VM´s (***start***) ou de Desligar VM´s (***stop***)

![alt text](https://github.com/osanam-giordane/MVP-Osanam-GIT/blob/master/Powershell/AZURE/Runbook_Automation/Start_Stop_VM/multiple_vms/images/campos.png?raw=true)
