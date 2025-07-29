# Comandos condutores para saída do terminal:

---

- Condutor `>`
  
  - Redireciona a saída de um comando para um arquivo, não mostrando a saída.
  
  - Exemplo: `ifconfig > interfaces.txt`

---

- Condutor `>>`
  
  - Redireciona a saída de um comando para um arquivo, mostrando a saída.
  
  - Exemplo: `sudo systemctl list-units | grep failed`

---

- Condutor `|`
  
  - Redireciona um comando para outro.
  
  - Exemplo: `sudo systemctl list-units | grep failed`

---

- Condutor `2>`
  
  - Redireciona a saída de erro de um comando para um arquivo, não mostrando a saída.
  
  - Exemplo: `if congif 2> erros.txt`

---

- Condutor `grep`
  
  - O `grep` ajuda a pegar algum conteúdo que você queira selecionar.
  
  - Exemplo: `ifconfig | grep "inet"`

---

- Condutor `cut`
  
  - O `cut` ajuda a cortar informações que você não queira.
  
  - Exemplo: `sudo apt list --upgradable | cut -d "/" -f1`
