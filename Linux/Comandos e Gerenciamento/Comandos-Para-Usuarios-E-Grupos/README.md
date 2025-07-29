# Gerenciando Usuário e Grupos

### Informações importantes:

- `/etc/passwd` --> Arquivo onde ficam salvos os usuário do Linux,

- `/etc/shadow` --> Arquivo onde ficam os hashes das senhas no Linux,

- `/etc/group` --> Arquivo onde ficam salvos os grupos do Linux,

- `useradd` --> Comando para adicionar um usuário no Linux,

- `adduser` --> Comando mais amigável para adicionar um usuário no Linux,

- `userdel` --> Comando para deletar um usuário no Linux,

- `deluser` --> Comando mais amigável para deletar um usuário no Linux,

- `groupadd` | `groupdel` --> Comandos para adicionar ou deletar um grupo no Linux,

- `usermod` --> Comando para modificar configurações dos usuários no Linux.

---

### Exemplos e Explicações:

- `useradd`:
  
  - Exemplo: sudo useradd pedro
  - Explicação: Esse comando vai apenas criar o usuário, sem criar a pasta home dele ou atribuir uma senha. Tendo que fazer o resto do processo com o `mkdir` e o `passwd`.

- `adduser`:
  
  - Exemplo: sudo adduser pedro
  
  - Explicação: Esse comando cria o usuário e faz todo pós processo de criação do usuário automaticamente.

- `userdel`:
  
  - Exemplo: sudo userdel pedro
  
  - Explicação: Esse comando no mesmo esquema do `useradd`, ele deleta apenas o usuário. Sem deletar o grupo do usuário, pasta home e etc.

- `deluser`:
  
  - Exemplo: sudo deluser pedro
  
  - Explicação: Esse comando no mesmo esquema do `adduser`, ele deleta o usuário fazendo todo o pós processo de deleção automaticamente.

- `groupadd`:
  
  - Exemplo: sudo groupadd Admins
  
  - Explicação: Esse comando vai adicionar um grupo interno no sistema, sem adicionar nenhum usuário dentro ou permissões específicas.

- `groupdel`:
  
  - Exemplo: sudo groupadd Admins
  
  - Explicação: Esse comando vai deletar o grupo do sistema, porém, você vai precisar retirar os usuário que estão dentro do grupo primeiro, depois ele vão conseguir deletar.

- `usermod`:
  
  - Exemplo: sudo usermod -s /usr/bin/zsh pedro
  
  - Explicação: Esse comando em específico, vai mudar o terminal do usuário pedro para o zsh. Esse comando tem vários usos, digite usermod -h para ver todos os usos.

- `/etc/passwd`:
  
  - Exemplo: `pedro:x:1001:1001::/home/pedro:/bin/zsh`
  
  - Explicação: Essa linha representa o usuário pedro, no arquivo passwd. Indicando o usuário, as informações do usuário, o ID do usuário, a pasta home dele e o terminal que ele está usando, nessa ordem. Você pode adicionar um usuário apenas editando o arquivo passwd, porém não é recomendado fazer desse jeito, pois pode ocorrer problemas no sistema se digitado errado.

- `/etc/group`:
  
  - Exemplo: `Admins: x:1001:ggoncalves,kali`
  
  - Explicação: Essa linha representa o grupo Admins, no arquivo group. Indicando o grupo em questão, informações do grupo, o ID do grupo e os usuários incluídos no grupo, nessa ordem. No mesmo esquema do passwd, você pode criar um grupo apenas editando o arquivo group, mas novamente, não é recomendado fazer desse jeito.

- `/etc/shadow`:
  
  - Exemplo: `ggoncalves:$y$j9T$NdrhmzoauxCxkqC4osWCo0$Z/Mx1uyKvraTjij9Kcir4XaKXlUVITV8xOJUDKdGbRA:20149:0:99999:7:::`
  
  - Explicação: Essa linha representa da senha em hash do usuário ggoncalves, no arquivo shadow. No mesmo esquema dos arquivos anteriores, você pode mudar a senha de um usuário editando o arquivo shadow, porém, novamente não é recomendado fazer desse jeito e para fazer assim, precisaria coloca a senha já criptografada no arquivo.
