# BackDoor

### Descrição:

#### 1: Remote_BackDoor.ino:<br>
Cria uma conta com privilégios de administrador com o nome "blanka" e senha "Ping@123". Também a oculta na tela de login e ativa a área de trabalho remota para ser acessível de um local remoto.

**Testado em:**<br>
**Sistema Operacional:** Windows 10<br>
**Usuário:** Usuário Administrador<br>
**Hardware:** ATtiny85 (Chinês)

#### 2: GoodOl' BackDoor.ino:<br>
Baseado na antiga técnica de backdoor do Sticky Keys, adicionando uma chave de registro em vez de substituir o arquivo no diretório system32. Após a execução bem-sucedida, pressione shift 5 vezes na tela de login e o prompt de comando aparecerá com privilégios de administrador.

Para remover a backdoor, execute o seguinte comando no prompt de comando com privilégios de administrador e a backdoor será removida.

***REG DELETE "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Image File Execution Options\sethc.exe***


**Testado em:**<br>
**Sistema Operacional:** Windows 10/7<br>
**Usuário:** Usuário Administrador<br>
**Hardware:** ATtiny85 (Chinês)
