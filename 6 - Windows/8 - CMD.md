# Command Line Windows

- `ver`: exibe a versão do windows
- `set`: exibe as informações de diretorio
- `cls`: limpa o terminal
- `systeminfo`: lista informações do sistema
- `help`: exibe ajuda para comandos especificos

## Network Troubleshooting

- `ipconfig` e `ipconfig /all`: visualiza informações de rede
- `ping ip/site`: serve para conferir o funcionamento do server
- `tracert ip`: rastreia a rota de internet até o alvo escolhido
- `nslookup`: analisa host e exbie ip
- `netstat`: mostra as conexões de rede atuais e as portas
  - `-a`: exibe todas as conexões estabelecidas e as portas abertas
  - `-b`: exibe o programa associado com cada porta
  - `-o`: exibe o PID de cada conexão
  - `-n`: exibe a forma numerica dos endereços e portas

## Gerenciamento de arquivos e disco

### Diretorios

- `cd`: sem parametros exibe o path atual, mas pode ser usado para caminhar entre as pastas
- `dir`: exibe diretorios da pasta atual
  - `/a`: exibe arquivos e pastas escondidos
  - `/s`: exibe todos os arquivos e todos os subdiretorios
- `mkdir nome-da-pasta`: serve para criar nova pasta
- `rmdir nome-da-pasta`: deleta uma pasta

### Arquivos

- `type`: exibe o tipo do arquivo
- `copy`: permite copiar o conteudo de um arquivo para outro
- `move`: serve para mover um arquivo de um lugar pro outro
- `del ou erase`: apaga arquivo

## Tasks e gerenciamento de processos

- `tasklist`: exibe os processos rodando
  - `tasklist /FI "imagename eq processo"`: filtra o processo pelo nome
- `taskkill /PID pid-do-processo`: encerra tarefa
- `shutdown`: encerra algum processo ou tarefa

### Outros comandos

- `chkdsk`: confere os discos de armazenamento
- `driverquery`: exibe a lista de drivers
- `sfc /scannow`: scaneia arquivos corrompidos e repara
- `comando /?`: exibe ajuda
- `more`: exibe arquivos de texto