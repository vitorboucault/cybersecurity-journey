# Processos em Linux

Processos são os programas rodando na máquina. São gerenciados pelo Kernel e cada um possui um ID

## Visualizando processos

- `ps`: exibe os processos que estão rodando pelo usuário, junto com o PID
- `ps aux`: exibe todos os processos rodando no servidor/maquina
- `top`: mostra estatisticas em tempo real sobre os processos

## Gerenciando processos

É possível enviar comandos que encerram processos.

- `kill <PID>`: mata processo desejado
- `SIGTERM`: Mata o processo mas permite que ele limpe tarefas
- `SIGKILL`: Mata o processo mas não faz nenhum cleanup
- `SIGSTOP`: Para ou suspende um processo

## Iniciando/Parando processos no Boot



- `systemctl <opçao> <servico>`: comando para interagir com o processo systemd

O comando `systemctl` possui 5 opções:

- Start
- Stop
- Enable
- Disable
- Status

## Processos no Background e Foreground


