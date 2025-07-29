# Gerenciando Redes

### Informações importantes:

---

### Comandos utilizados:

- `route` --> Comando utilizado para criação, edição e visualização de rotas e tabelas de roteamento.

- `ifconfig` --> Comando utilizado para criação, edição e visualização de interfaces de rede.

- `netstat` --> Comando para verificação de conexões ativas, portas abertas, serviços ativos e etc.

- `ping` e `traceroute` --> Comandos para testes de conectividade de rede, utilizando o protocolo ICMP.

- `ip` --> Comando utilitário que vem por padrão configurado nos sistemas Linux.

---

### Exemplos e Explicações:

- `route`:
  
  - Exemplo: route -n
  
  - Explicação: Esse comando em especifico mostra a tabela de roteamento do computador, mostrando ip de destino, gateway, mascara de sub-rede, algumas métricas e a interface de rede por onde o tráfego está saindo.

- `ifconfig`: 
  
  - Exemplo: ifconfig -a
  
  - Explicação: Esse comando mostra as interfaces de rede do servidor e seu detalhes como: Nome da interface (eth0, eth1, etc), MTU (1500), inet (10.151.48.135), inet6 (fe80::3cf8:b30c:6ea1:f99b) e mais.

- `netstat`:
  
  - Exemplo: netstat -nat
  
  - Explicação: Esse comando puro `netstat`, ele mostra a conexões em funcionamento no servidor, assim como IP, Porta, Status, Protocolo e etc. Porém com o `-nat` ele consegue filtrar pelos serviços que estão abertos.

- `traceroute`:
  
  - Exemplo: traceroute google.com
  
  - Explicação: Esse comando exibe todo caminho trafegado do servidor até o google.com. Resolvendo endereços DNS de dispositivos pelo caminho.

- `ip`:
  
  - Exemplo: ip a
    
    - Explicação: Esse comando faz a mesma coisas que o `ifconfig`, porém, mais compacto.
  
  - Exemplo: ip -h -s link
    
    - Explicação: Esse comando mostra algumas informações a respeito da placa de rede, como: MAC Address, MTU, UpDown, Estatisticas e etc. Mas de uma forma mais organizada humanamente.
