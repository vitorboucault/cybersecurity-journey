# Baixando arquivos (Wget)

- `wget <link>`: comando para baixar arquivos

## Transferindo arquivos do Host - SCP (SSH)

Comando que permite transferir arquivos entre 2 computadores utilziando o protocolo SSH que fornece autenticação e criptografia.

- `scp important.txt ubuntu@192.168.1.30:/home/ubuntu/transferred.txt`: comando envia arquivo para uma outra maquina
- `scp ubuntu@192.168.1.30:/home/ubuntu/documents.txt notes.txt`: copia arquivo de uma outra maquina remota.

## Arquivos de Server do Host

- `python3 -m  http.server`: comando para criar um server no host