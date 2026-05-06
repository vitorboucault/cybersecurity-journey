# Active Directory

O `Windows Domain` serve para administrar um grupo de usuários e computadores debaixo de um administração de um negócio.

A ideia principal é centralizar a administração de componentes comuns de uma rede de computadores Windows em um único repositóio chamado `Active Directory`.

O servidor que roda o Active Directory é conhecido como `Domain Controller`

## Active Directory Domain Service

Atua como um catalogo que segura a informação de todos os objetos que existem na sua rede.

Objetos como: usuários, grupos, maquinas, impressoras, shares e vários outros.

### Users

São objetos conhecidos como entidades de segurança, então ele podem ser autenticados pelo dominio e receber privilégios.

Podem ser representados por dois tipos de entidades:

- `Pessoas`: usuarios que geralmente representam pessoas na organização que precisam acessar a rede, como colaboradores.
- `Serviços`: usuarios também podem ser definidos como serviço tipo MSSQL. Cada serviço precisa de um usuário para rodar, mas são diferentes de usuários regulares, por que eles só vão os privilégios especificos para rodar o serviço específico.

### Machines

Cada computador que entra no AD Domain, um objeto de maquina é criado.

Para identificar as contas de maquina é relativamente facil, eles tem o nome seguido de um $, por exemplo: `DC01` vai se chamar `DC01$`

### Security Groups

Você pode adicionar máquinas ou usuarios aos grupos e eles já vão herdar os privilegios preestabelecidos do grupo.

Grupo importantes em um domain:

- `Domain Admins`: Usuários do grupo tem privilegio de admin.
- `Server Operators`: Usuarios podem administrar o Domain Controller, mas não podem mudar nenhum grupo administrativo
- `Backup Operators`: Users podem acessar qualquer arquivo, ignorando sua permissão, são usados para realizar os backups de dados nos computadores.
- `Account Operators`: Podem modificar ou criar contas no domain
- `Domain Users`: Inclui todos as contas de usuarios no dominio
- `Domain Computers`: Inclui todos os computadores no dominio
- `Domain controllers`: Inclui todos os DCs no domain

### Active Directory Users And Computers

São divididos em `Organizational Units (OUs)`.

Cada usuário só pode fazer parte de um OU de cada vez.

### Group Policie Objects

São grupos de políticas para os OUs, onde cada um possui suas regras. Eles são gerenciados pelo `Group Policy Management`

### Authentication Methods

Dois protocolos são usados para autenticação de rede nos windows domains:

- `Kerberos`: Protocolo padrão em qualquer domain recente
- `NetNTLM`: Protocolo de autenticação legado, mantido por motivos de compatibilidade

