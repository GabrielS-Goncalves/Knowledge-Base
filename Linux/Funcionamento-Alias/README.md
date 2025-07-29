# Informações Alias

## Conceito:

O uso de alias no Linux é importante para facilitar o uso do sistema como um todos. Pois podemos substituir comandos muitos grandes em comandos pequenos.

---

## Comandos/Arquivos utilizados:

- alias - Utilizado para criar um comando personalizado no Linux.

- `~/.bashrc` - Arquivo de configuração do bash no Linux.

- `~/.bash_alaiases` - Arquivo com os alias criados pelo usuário de maneira permanente.

---

## Procedimento:

Comando para adicionar um Alias (Porém, o Alias criado assim se perde quando o terminal fecha):

- alias (Alias desejado)="Comando desejado"

Para que o comando fique permanentemente, alguns passos são necessários:

- Ir para a pasta do usuário.

- Editar o arquivo `.bash_alaiases` (nano `.bash_alaiases` ou vi `.bash_alaiases`).

- Digitar o alias a ser criado, com a sintaxe acima e salvar o arquivo.

- Digite o comando: `source .bashrc` para salvar os alias permanentemente.

---

## Exemplos:

- ifaces (Comando: ifconfig Eth0 | grep "inet" )
  
  - Mostra os ips da placa de rede Eth0

- usr (Comando: Whoami)
  
  - Mostra o usuário logado
