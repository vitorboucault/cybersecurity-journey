# Configuração do Sistema

MSConfig é utilizado para troubleshooting avançado e é utilizado para ajuda a diagnosticar problemas.

Dentro dele existem 5 abas:

- `General:` selecionos serviços e dispositivos que o Windows carrega após o boot
- `Boot:` pode definir várias opções de boot para o S.O
- `Services:` lista os serviços configurados para o sistema mesmo estando em execução ou parado.
- `Startup`
- `Tools

# Configurações avançadas do sistema

O windows permite que você configure e controle o comportamento da performance e a recuperação do sistema.

- Para acessar essa parte podemos procurar em: `View advanced system settings`
- A parte `Startup and Recovery` mostra informaçÕes para debug, que mostra o tipo do crash dump (desepejo de memoria) configurado para o sistema

No Windows existem diferentes tipos de dump como:

- Automatic memory dump
- Kernel memory dump
- Small memory dump (256kb)
- Complete memory dump
- None

## Computer Management

Ferramenta do painel System Configuration

Computer Management `compmgmt` tem 3 seções primárias:

- System Tools
- Storage
- Services and applications

### System Tools

O `Task Scheduler` cria e gerencia tasks comuns que o computador pode fazer automaticamente de acordo com a quantidade de tempo que estipularmos

Para criar uma tarefa básica é só:

- Clicar em `Criate Basic Task` embaixo de `Action`

#### Event Viewer

Permite que a gente visualize os eventos que ocorreram no computador.

Existem 3 paineis

1. `Custom View` fornece uma lista hierarquica em arvore dos logs de eventos
2. `Windows Logs` fornece um overview geral dos eventos
3. E o outro é o painel de ações

#### Shared Folders

Lista onde se vê as pastas que são compartilhadas que outros podem conectar também

Em `Shares` está a share padrão do windows, C:/ e a ADMIN$.

Em `Sessions` voce pode ver a lista de usuarios conectados atualmente nas shares.

Em `Open Files` estãos as pastas e/ou arquivos que estão conectadas aos usuários.

#### Performance Monitor

Usado para visualizar os dados de perfomance em tempo real ou um log file.

#### Device Manager

Nos permite visualizar e configura o hardware.

#### Storage

Dentro deles está o `Windows Server Backup` e o `Disk Management`

Disk Managemente você consegue realizar tarefas avançadas de armazenamento como:

- Setar um novo drive
- Extender uma partição
- Reduzir uma partição
- Atribuir ou alterar uma letra de unidade

#### Services and Applications

Mostra o todos os serviços e status clicando no botão `Services`

## System Information

System Information `msinfo32` que reune informações sobre o computador e mostra de maneira fácil o hardware, componente do sistema, e o ambiente do software.

Ele é dividido em 3 seções:

- `Hardware Resources`
- `Component`
- `Software Environment`

## Resource Monitor

Resource monitor (`resmon`) exibe por processos e de forma agregada informações como uso de CPU, memoria, disco e rede.

## Command Prompt

O `cmd` serve para rodar alguns prompts de comando como:

- `hostname`: exibe o nome do computador
- `whoami`: exibe o nome do usuario logado
- `ipconfig`: exibe as configurações de rede do computador

Todo comando possui um manual para ajuda no windows, e comando é:

- `/?`: para pedir ajuda no `cmd` do Windows

O comando para limpar a tela do `cmd` é:

- `cls`: para limpar a tela

O comando para ver estatisticas do protocolo e as atuais conexões TCP/IP é:

- `netstat`: também algumas flags (parametros) podem ser usados
- `net`: usado para gerenciar recursos de rede
