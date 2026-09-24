# Chat TCP/IP - Redes de Computadores

Projeto de implementação de uma arquitetura Cliente-Servidor multithread utilizando Sockets em Java puro.

## Estrutura do Projeto
- `Servidor.java`: Gerencia as conexões, identifica o IP local e atua como host principal.
- `ClienteHandler.java`: Processa as lógicas de salas, broadcast e salvamento de logs em arquivos `.txt`.
- `Cliente.java`: Interface de texto do usuário que envia comandos e escuta a rede simultaneamente.

## Como compilar
Os arquivos foram desenvolvidos para rodar no terminal do Linux (Debian). Abra o terminal nas respectivas máquinas e execute os comandos de compilação:

**No Servidor:**
javac Servidor.java ClienteHandler.java

**No Cliente:**
javac Cliente.java

## Como executar
1. Inicie o servidor primeiro executando:
java Servidor

2. O servidor exibirá o seu IP na tela e pedirá para definir a porta (ex: 5000).
3. Inicie os clientes executando:
java Cliente

4. Insira o IP exibido pelo servidor, a porta escolhida e um nome de usuário.
5. Digite `/help` no cliente para visualizar a lista de comandos (como `/join #sala`).
