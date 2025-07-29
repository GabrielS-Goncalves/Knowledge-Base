# Gerenciando Processos

### Informações importantes:

- Um processo é um programa/tarefa que está sendo executado no SO,

- Todo processo possui um PID (Process ID) que o identifica no sistema,

- Muitas vezes um processo pode estar travado ou causando problemas,

- Os processos podem ser divididos em `Foregroud` e `Background`:
  
  - `Foreground`: São processo que estão rodando na tela,
  
  - `Background`: São processo que estão rodando por debaixo dos panos.

- Um processo pode iniciar outros chamados de `Sub-processos`,

- Os estado básicos de um processo são: `Running`, `Stopped`, `Sleeping` e `Zombie`.

---

### Comandos utilizados:

- `ps` --> Esse comando serve para verificar processos, padrão na maioria dos Linux,

- `top` --> Esse comando funciona igual o `ps`, mas com uma visualização mais informativa.

- `htop` --> Esse comando tem o mesmo propósito dos anterior, mas com gerenciamento melhorado, normalmente não vem por padrão, tendo que instalar.

- `kill` --> Esse comando serve para matar processos no sistema.

- `jobs` --> Esse comando serve para listar os processos suspensos no sistema.

- `fg` --> Esse comando serve para trazer um processo do `Backgroud` para o `Foregroud`.

---

### Exemplos e Explicações:

- `ps`
  
  - Exemplo: ps -aux | grep "firefox"
  - Explicação: Esse comando acima vai tirar uma "foto" de todos os processos de todos usuários e com o apoio do `grep` ele vai filtrar todos o processos que contenham "firefox" neles.

- `kill`
  
  - Exemplo: kill 317844
  - Explicação: Esse comando acima vai matar o processo em questão (era do firefox) detalhe que para usar o `kill` você precisa obrigatoriamente do PID associado ao processo em questão, o nome não vai funcionar.
