# Caracteres coringas do Linux

---

#### Utilidade:

- São usados para representar um ou mais caracteres.

- São úteis para realizar operações em massa (Listar, Deletar, Etc).

---

#### Caracteres:

- `*`:
  
  - Representa qualquer sequencia de caracteres em sequência.
  
  - Exemplo: ls -l *.txt
  
  - Extra: Vai aparecer todos os arquivos dá pasta com o final `.txt`.

- `?`:
  
  - Representa qualquer caractere único.
  
  - Exemplo: ls -l script?.sh
  
  - Extra: Vai aparecer todos os arquivos dá com o final `.sh`, porém, somente aqueles com números do lado do T, por exemplo: script1.sh, script2.sh, script3.sh e etc.

- `[]`:
  
  - Representa um conjunto ou intervalo de caracteres.
  
  - Exemplo: ls -l file[0-4].txt
  
  - Extra: Ele vai listar todos o arquivos `.txt` na pasta, mas somente de 0 até 4. Ele só lê até o 9. Para mais: `ls -l file[0-9]*.txt`, assim ele vai selecionar qualquer coisa além do range.
