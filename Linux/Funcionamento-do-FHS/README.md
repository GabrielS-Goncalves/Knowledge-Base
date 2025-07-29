# Funcionamento do FHS

### Linux FHS (Filesystem Hierarchy Standart)

---

#### O que é o FHS no Linux?

- Ele é uma padronização de organização, para o sistema de diretório do projeto GNU Linux.

- Assim facilitando muito a `Interoperação` e `Administração` do sistema. Onde a maioria das distribuições Linux seguem esse padrão.

#### Como é o padrão de diretórios?

- / --> Diretório base do sistema Linux (Raiz). O ponto de início de toda a árvore de diretórios. Todas as outras pastas estão subordinadas a este diretório.

- /bin --> Diretório reservado para arquivos binário do sistema (Programas, comandos, executáveis e etc...). Contém os executáveis essenciais acessíveis a todos os usuários. Exemplos: `ls`, `cp`, `mv`.

- /boot --> Diretório reservado para arquivos de boot do sistema (Kernel Linux). Arquivos necessários para a inicialização do sistema, incluindo o `kernel`, `initrd` e arquivos de configuração do `bootloader`.

- /dev --> Diretório reservado para arquivos de hardware (Disco do sistema, compartilhamentos e mais). Arquivos de dispositivo que representam hardware e periféricos do sistema. Exemplos: `sda` (disco rígido), `tty` (terminais).

- /etc --> Diretório reservado para arquivos de configuração (Serviços, aplicações, sistema e etc...). Arquivos de configuração global do sistema. Aqui estão as configurações que afetam todo o sistema e todos os usuários.

- /home --> Diretório reservado para arquivos de usuário (Documentos, downloads, Musicas e etc...). Diretórios pessoais dos usuários. Cada usuário possui uma pasta aqui para seus arquivos pessoais. Exemplo: `/home/ggoncalves`.

- /lib e /lib64 --> Bibliotecas compartilhadas essenciais para os binários em `/bin` e `/sbin`.

- /media --> Ponto de montagem para mídias removíveis como CDs, DVDs e pen drives.

- /mnt --> Diretório usado temporariamente para montagem de sistemas de arquivos.

- /opt --> Pacotes de aplicativos opcionais e adicionais. Softwares personalizados ou de terceiros podem ser instalados aqui.

- /proc --> Sistema de arquivos virtual que fornece informações sobre processos e recursos do sistema.

- /root --> Diretório home do usuário root (administrador).

- /sbin --> Binários essenciais do sistema destinados ao administrador. Exemplos: `iptables`, `ifconfig`, `reboot`.

- /srv --> Dados específicos de serviços oferecidos pelo sistema. Por exemplo, páginas web em um servidor Apache.

- /tmp --> Arquivos temporários usados por aplicativos.

- /usr --> Hierarquia secundária para dados de usuários. Contém a maioria dos utilitários e aplicativos de usuário.
  
  - `/usr/bin`**:** Binários não essenciais para o sistema, mas disponíveis para todos os usuários.
  - `/usr/lib`**:** Bibliotecas para os binários em `/usr/bin` e `/usr/sbin`.
  - `/usr/local`**:** Dados locais específicos da máquina. Uma boa área para instalar programas compilados manualmente.
  - `/usr/sbin`**:** Binários não essenciais do sistema destinados ao administrador.

- /var --> `/var`**:** Arquivos de dados variáveis, como logs, bancos de dados e filas de e-mails.
  
  - `/var/log`**:** Arquivos de log do sistema e aplicações.
  - `/var/spool`**:** Dados em espera para processamento, como filas de impressão ou e-mails pendentes.
  - `/var/www`**:** Raiz padrão para documentos web em servidores HTTP.
