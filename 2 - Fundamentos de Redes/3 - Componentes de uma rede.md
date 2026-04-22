# Componentes de uma Rede

## Dispositivos Finais

Conhecidos também como host, é qualquer dispositivo que em última instância, acaba enviando ou recebendo dados dentro de uma rede.

Computador, celular, tablet, dispositivos IoT…

Eles servem como a interface de usuário primario para a web, permitindo usuários acessarem os recursos e serviços da internet de forma contínua, via Ethernet ou Wi-fi.

Dispositivos Intermediários

Tem como único papel em facilitar o fluxo de dados entre os dispositivos finais, em uma LAN ou entre diferentes redes.

São roteadores, switch, modens e pontos de acesso, dispositivos que tem o papel de garantir a transmissão de dados de forma eficiente e segura. São responsáveis pelo encaminhamento de pacotes, direcionado os pacotes de dados para os seus destinos lendo as informações de endereço de rede e determinando o caminho mais eficiente. Eles conectam as redes e controlam o tráfego para melhorar a performance e confiabilidade.

Gerenciando o fluxo de dados com protocolos, eles garante transmissões tranquilas e previnem a congestão.

Dispositivos intermediários incorporam recursos de segurança como firewall para proteger as redes de acessos não autorizados e ameaças potenciais.

Operando em diferentes camadas do modelo OSI, roteadores na camada 3 e switches na camada 2, utilizam tabelas de roteamento e protocolos para tomar decisões fundamentadas sobre o encaminhamento de dados.

Um exemplo comum é uma rede de casa, onde o dispositivo intermediários como um roteador conecta todos os aparelhos domésticos a internet.

## Network Interface Cards

É um componente de hardware instalado em um computador, ou outro dispositivo, que habilita a conexão a uma rede.

Cada NIC possui um endereço MAC unico, que é essencial para os dispositivos se identificarem entre si, facilitando a conexão com a camada data link.

Podem ser desenvolvidos para conexão via cabo Ethernet ou wi-fi.

## Roteadores (Routers)

É um dispositivo intermediario que tem um papel importante de encaminhar os pacotes de dados entre as redes, e direciona também o tráfego de internet.

Operando na layer 3 do modelo OSI, eles leem a informação do endereço de rede nos pacotes de dados e determinam os seus destinos.

Utilizam protocolos como OSPF (open shortest path first) ou BGP (border gateway protocol) para encontrar o caminho mais eficiente para os dados navegarem pelas redes interconectadas, incluindo a internet.

Eles preenchem esse papel examinando os pacotes de dados que chegam e que vão ser enviados para os seus destinos, baseado no endereço IP. Conectando múltiplas redes, roteadores e permitindo os dispositivos se comunicarem em diferentes redes.

Eles também fazem o gerenciamento do tráfego selecionando os caminhos ideias para a transmissão de dados, o que previne a congestão.

Os roteadores aumentam a segurança com recursos como firewalls e listas de controle de acesso.

## Switches

O papel principal é conectar múltiplos dispositivos na mesma rede.

Operam na camada data link (2) e network layer (3) do modelo OSI.

Entretanto, os que operam na layer 2 não operam 3.

Eles utilizam o endereço MAC para encaminhar dados ao destinatário pretendido.

Eles permitem que computadores, impressoras e servidores se comuniquem diretamente entre si por meio da rede.

## Cabos e Conectores

Materiais físicos usados para conectados os dispositivos em uma rede.

## Network Protocols

São o conjunto de regras e convenções que controlam como o dado vai ser formatado, transmitido, recebido e interpretado ao longo da rede.

Eles abrangem uma gama de aspectos como: 
1. Segmentação de dados
2. Endereçamento
3. Roteamento
4. Check de erros
5. Sincronização

Protocolos de rede comum incluem: 
1. TCP/IP
2. HTTP/HTTPS
3. FTP
4. SMTP

## Network Management Software

Consiste nas ferramentas e aplicações usadas para monitorar controlar e manter componentes de rede e operações.

Essas soluções de software oferecem: 
1. Monitoramento de perfomance
2. Gerenciamento de configurações
3. Analise de falhas
4. Gerenciamento de segurança

Ajuda os administradores da rede a garantir que a rede vai operar de forma eficiente.

**Software Firewalls**

Aplicações de segurança instaladas nos computadores individuais ou dispositivos que monitoram e controla trafego de entrada e saída na rede, baseada em regras de segurança predeterminadas.

**Servidores**

Computadores poderosos que fornecem serviços a outros computadores através de uma rede. Eles são como a espinha dorsal dos sites, emails, arquivos e aplicações.

Eles tem um papel crucial hospedados os serviços aos quais os clientes tem acesso, facilitando a prestação de serviço.

Permitem compartilhamento de recursos para múltiplos usuários e gerenciamento de dados. Também gerenciam a autenticação controlando os acessos e permissões dos usuários.
