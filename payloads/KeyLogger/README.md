# KeyLogger

### Descrição:

#### 1: TimeBomb_KeyLogger.ino:<br>
Um Keylogger baseado em PowerShell. Funciona ao depositar o payload em um diretório temporário e executá-la em segundo plano. Registra as teclas pressionadas por um tempo determinado. 
Após o término do tempo, envia as teclas registradas para o webhook.site e exclui todos os dados do keylogger do diretório temporário. <br>Por favor, observe que agora é detectável pela maioria dos programas antivírus. A única maneira de torná-lo indetectável é ofuscar o payload.<br>

**Instruções:**<br>
Antes de usar, certifique-se de que o gancho do WebHook.site está definido na carga útil do keylogger, que você encontrará quase no final do script. Além disso, o 
tempo atual está configurado para 1 minuto; você pode aumentar o tempo conforme necessário em ".AddMinutes(-1)", que você também encontrará perto do local do webhook.<br>

**Testado em:**<br>
**Sistema Operacional**: Windows 10|8|7<br>
**Usuário**: Usuário Administrador/Normal<br>
**Limitações**: Política de Execução, Antivírus :p<br>
**Hardware**: ATtiny85 (Chinês)
