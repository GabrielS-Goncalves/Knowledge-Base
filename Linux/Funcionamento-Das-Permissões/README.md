# Gerenciando Permissões

### Informações importantes:

- Permissões servem para controlar o acesso a arquivos e pastas no Linux,

- As permissão são baseadas nos usuário e grupos do Linux,

- No Linux nós temos basicamente basicamente as permissões: `Read`, `Write` e `Execution`,

- Também existem algumas permissões especiais como: `Setupid`, `Setgid` e `Sticky Bit`.

- `Read (r)` --> Permite ler um arquivo ou listar uma pasta,

- `Write (w)` --> Permite modificar um arquivo ou algo em uma pasta,

- `Execution (x)` --> Permite executar um arquivo ou acessar um pasta.

---

### Comandos utilizados:

- `chmod` --> Comando para alterar as permissões,

- `chown` --> Comando para alterar o dono,

- `chgrp` --> Comando para alterar grupo.

---

### Exemplos e Explicações:

- `Read (4)`, `Write (2)` e `Execution (1)`:
  
  - Exemplo: sudo chmod 600 /etc/sssd/sssd.conf
  
  - Explicações: Esse comando em especifico atribui a permissão de `Read` e `Write` somente para o dono do arquivo sssd.conf. Para cada permissão existe um numero, para dar permissão máxima você pode usar o 7 (4+2+1), ele equivale ao rwx.

- `chmod`:
  
  - Exemplo: sudo chmod 770 /var/log
  
  - Explicação: Esse comando em especifico atribui as permissões de `Read`, `Write` e `Execulte` para o usuário e grupo dono da pasta log, deixando os outros sem permissão nenhuma.

- `chown`:
  
  - Exemplo: sudo chown root:root /var/log
  
  - Explicação: Esse comando em específico muda o dono da pasta log para o usuário root e para o grupo root.

- `chgrp`:
  
  - Exemplo: sudo chgrp root /var/log
  
  - Explicação: Esse comando em específico muda o grupo da pasta log para root.
