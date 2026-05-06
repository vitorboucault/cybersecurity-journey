# PowerShell

## Sintaxe Básica:

É utilizada a convenção `Verb-Noun`. Então `Verb` determina a ação e `Noun` o objeto.

Os comandos do PowerShell são chamados de: `cmdlets`

### Basico do Cmdlets

O comando `Get-Command` exibe todos os comandos do PowerShell

- Para filtrar podemos utilizar `-CommandType "Function“`

- `Get-Help Comando-Escolhido`: Para conseguir ajuda sobre o comando

- `Get-Alias`: lista os comandos alias utilizados para simplificar alguns comandos 

### Navegando entre os arquivos

- `Get-ChildItem`: funciona como o ls ou o dir
- `Set-Location -Path ".\Documents"`: para navegar entre as pastas
- `New-Item -Path ".\captain-cabin\captain-wardrobe" -ItemType "Directory"`: serve para criar um novo arquivo ou pasta
- `Remove-Item -Path ".\captain-cabin\captain-wardrobe\captain-boots.txt"` remove arquivo ou pasta
- `Copy-Item`: serve para copiar arquivo
- `Remove-Item` serve para deletar arquivo
- `Get-Content`: para exibir arquivos

### Piping e Filtrando dados

- `|` É utilizado o pipe para encaminhar o resultado de um comando para outro
- Existe também os operadores de comparação:
  - `-ne`: nao igual (!=)
  - `-gt`: maior que (>)
  - `-ge`: maior que ou igual a (>=)
  - `-lt`: menor que (<)
  - `-le`: menor que ou igual a (<=)

### Dados de rede e sistema

- `Get-ComputerInfo`: exibe informações do computador
- `Get-LocalUser`: exibe todas as informações dos usuários locais no sistema
- `Get-NetIPConfiguration`: similar ao comando ipconfig
- `Get-NetIPAddress`: Exibe detalhes dos endereços IP conectados a rede

### Analise do sistema em tempo real

- `Get-Process`: ferramenta para monitoramento, exibe informações importantes como os processos rolando, uso de cpu etc
- `Get-Service`: exibe os processos na maquina
- `Get-NetTCPConnection`: para monitorar conexões de rede ativas
- `Get-FileHash`: usado para gerar arquivos hash, importante para resposta a incidentes

### Scripting

É o processo de escrever e executar uma serie de comandos em um bloco de texto.

- `Invoke-Command`: utilizado para executar os scripts
  - Exemplo: `Invoke-Command -ComputerName Server01 -Credential Domain01\User01 -ScriptBlock { Get-Culture }`

