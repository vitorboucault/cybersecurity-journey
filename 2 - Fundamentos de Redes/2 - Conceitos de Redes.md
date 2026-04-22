# Conceitos de Redes

## OSI Model

OSI significa Open Systems Interconnection, é um framework conceitual que padroniza as funções da telecomunicação ou sistema computacional, em 7 camadas:

1. Camada Física (Layer 1):
    1. É responsável por transmitir fluxos de bits brutos por meio de um meio físico.
    2. Lida com a conexão fisica entre dispositivos como: cabos Ethernet, hubs e repetidores.
2. Camada Data Link (Layer 2):
    1. Provê transferências de dados node-to-node. É como um link direto entre dois nodes conectados fisicamente.
    2. Dispositivos como switches e pontes, operam nessa layer utilizando endereços MAC (media access control) para identificar os dispositivos de rede.
   3. Existe uma peça de hardware que todo computador tem para se conectar em uma rede que é o NIC (network interface card) que vem com o endereço MAC
3. Camada de Rede (Layer 3):
    1. Responsável por encaminhar os pacotes, até por meio de diferentes roteadores, para chegar a rede de destino final
    2. Responsável pelo endereçamento lógico e determina o caminho, garantindo que os dados cheguem ao destino correto dentre várias redes.
    3. Roteadores operam nessa layer usando o endereços IP (internet Protocol) para identificar os dispositivos, e escolher o caminho mais eficiente para transmissão de dados.
   4. Esses protocolos utilizam o OSPF (Open Shortest Path First) e RIP (Routing Information Protocol)
4. Camada de Transporte (Layer 4):
    1. Essa camada provê serviços de comunicação ponta a ponta para as aplicações. Responsável pela entrega confiável ou não dos dados, segmentação, remontagem de mensagens, controle de fluxo e verificação de erros.
    2. Protocolos como TCP (Transmission Control Protocol) e UDP (User Datagram Protocol) funcionam nessa camada.
    3. TCP oferece uma transmissão confiável e orientada por conexão com recuperação de erros.
    4. Enquanto que o UDP provê uma comunicação mais rápida e sem conexão
5. Camada de Sessão (Layer 5):
    1. Gerencia sessões entre aplicações.
    2. Ela estabelece, mantém e encerra conexões, permitindo que os dispositivos mantenham comunicações contínuas, conhecidas como sessões.
    3. Essencial para pontos de verificação e recuperação de sessão, garantindo que os dados transferidos possa ser retomada sem interrupções.
    4. Protocolos e APIs operam nessa camada coordenando a comunicação entre sistemas e aplicações
   5. O termo correto para quando uma conexão é estabelecida com sucesso é session
6. Camada de apresentação (Layer 6):
    1. Atua como um tradutor entre a camada de aplicação e o formato da rede
    2. Ela lida com a representação dos dados, garantindo que a informação enviada pela camada de aplicação de um sistema possa ser lida pela camada de aplicação de outro.
    3. Isso inclui criptografia e decriptografia de dados e a conversão de formatos de dados.
    4. Protocolos de criptografia e técnicas de compressão de dados operam nessa camada para assegurar e otimizar a transmissão de dados
7. Camada de aplicação (Layer 7):
    1. Camada mais alta do modelo OSI
    2. Fornece serviços de rede diretamente as aplicações dos usuários finais
    3. Permite habilita compartilhamento de recursos, acesso remoto a arquivos e outros serviços de rede.
    4. Protocolos que operam nessa rede: HTTP para navegar na internet, FTP para transferência de arquivos, SMTP para transmissão de e-mails e DNS para resolução de nomes de domínios para endereço IP.
    5. Funciono como interface entre a rede e o software aplicativo

## Modelo TCP/IP

É um versão condensada do modelo OSI, concebido para aplicação prática na internet e em outras redes.

Existem 4 camadas no modelo TCP/IP: 
1. Link Layer
    1. Responsável por gerenciar os aspectos físicos do hardware de rede e media
    2. Inclui tecnologias como Ethernet, para conexões via cabo e wifi.
    3. Essa camada corresponde as camadas Fisica e de Ligação de dados do modelo OSI, abrangendo tudo de conexão fisica até a formulação de dados
2. Internet Layer
    1. Gerencia o endereçamento lógico de dispositivos e o roteamento de pacotes nas redes
    2. Protocolos como IP e ICMP operam nessa camada, garantindo que os dados cheguem ao destino pretendido, determinando caminhos lógicos para a transmissão de pacotes
    3. Corresponde a Network Layer (Layer 3) no modelo OSI
3. Transport Layer
    1. Fornece serviços de comunicação ponta-a-ponta que são essenciais para o funcionamento da internet.
    2. Inclui o uso do TCP para comunicação confiável, e UDP para comunicação rápida e serviços sem conexão.
    3. Essa camada garante que os pacotes de dado vão ser entregues em de forma sequencial e sem erros, correspondendo a Transport Layer do modelo OSI
4. Application Layer
    1. Contém protocolos que oferecem serviços específicos de comunicação de dados para aplicativos.
    2. Protocolos como: HTTP, FTP, SMTP permitem funcionalidades como navegar na internet, transferência de arquivos, e serviços de email.
    3. Essa camada corresponde as top 3 camadas do modelo OSI.

O modelo TCP/IP simplifica o modelo OSI combinando certas camadas. Ele é também mais orientado as aplicações, focando na necessidade real da comunicação de rede. Tornando ele mais efetivo para troca de dados pela internet, atendendo assim, as necessidades tecnológicas atuais. 

O TCP é "conection-based" onde ele precisa ter uma conexao entre cliente e dispositivo atuando como um servidor antes do envio do dado.

Por conta disso o protocolo garante que todos os dados enviados vão ser recebidos pela outra ponta. Esse processo é chamado de Three-Way handshake

### Frames e Pacotes

Pacote ou packet, é um pedaço de dado da camada 3 (Network Layer), e contém informações como:

- IP Header
- Payload

Um frame, no entanto é usado na layer 2 (Data Link) ele encapsula o pacote e adiciona informações como o endereço MAC.

Exemplo, uma imagem carregada em um site não é enviada para o seu computador por completo, mas sim pequenos pedaços que sao reconstruindos e exibidos no computador.

### TCP Packets

Eles contém um header ao enviar um pacote que o encapsulamento adiciona:

1. **Source Port**
2. **Destination Port**
3. **Source IP**
4. **Destination IP**
5. **Sequence Number**
5. **Acknowledgement Number**
6. **Checksum:** é o valor que fornece integridade ao TCP
7. **Data**
8. **Flag**

### Three-Way Handshake

É o termo de conexão entre dois dispositivos, eles comunicam-se usando as seguintes mensagens:

1. **SYN:** é o pacote com a mensagem inicial enviada pelo cliente
2. **SYN/ACK:** pacote enviado pelo dispositivo que recebe a primeira mensagem
3. **ACK:** pode ser usado tanto pelo cliente, quanto pelo servidor, para reconhecer a que a mensagem foi rceebida
4. **DATA:** quando ocorre a conexão, o dado é enviado
5. **FIN:** é usado para encerrar a conexão depois de compelta
6. **RST:** 

### TCP Encerrando Uma Conexão

O protocolo vai encerrar uma conexão quando reconhece que a parte final recebeu os todos os dados.

Para encerrar, o dispositivo vai enviar um pacote FIN para o outro dispositivo. Assim esse 2 dispositivo, devolve uma mensagem ACK e uma mensagem FIN para encerrar também.

## Modelo UDP/IP

Diferente do TCP, o protocolo UDP (**User Datagram Protocol**), não requer que dois dispositivos estejam conectados. Esse protocolo também é usado comumente em serviços que toleram perca de dados, como streaming e chat de voz.

Os pacotes do UDP possuem um header com as seguintes informações:

1. Time To Live (TTL)
2. Source IP Address
3. Destination IP Address
4. Source Port
5. Destination Port
6. Data

## Protocolos

São regras padronizadas que determinam a formatação e o processamento de dados  para facilitar a comunicação entre dispositivos em uma rede.

Esses protocolos operam em diferentes camadas nos modelos de rede, cada um deles projetado para lidar com tipos específicos de dados e de comunicação.

1. Protocolos comuns de internet:
    1. HTTP (Hypertext Transfer Protocol): Navegador de internet
    2. FTP (File Transfer Protocol): Facilita a transferência de arquivos
    3. SMTP (Simple Mail Transfer Protocol): Protocolo de envios de email
    4. UDP (User Datagram Protocol): Comunicação sem necessidade uma comunicação entre dispositivos, ideal para serviços de streaming.
    5. IP (Internet Protocol): Gerencia o endereçamento e roteamento dos pacotes de dados que vão viajar de um ponto a outro pelas redes.

## Transmissão

Processo de envio de sinais de dados de um dispositivo para o outro.

1. Tipo de transmissão:
    1. Analogica: utiliza sinais continuos para representar informações, sendo comum em rádios
    2. Digital: utiliza sinais discretos como bits para codificar os dados, normal em tecnologias modernas de comunicação como redes de computadores e telefones.
2. Modos de transmissão:
    1. Simplex: Apenas 1 caminho de comunicação, como um teclado para o computador
    2. Half-duplex: permite 2 caminhos de comunicação mas não simultâneos, como walkie-talkie.
    3. Full Duplex: usado em ligações de telefone, suporta comunicação bidirecional simultânea
3. Meios de transmissão:
    1. Meios físicos pelos quais os dados são transmitidos em uma rede que pode ser via cabo ou não.
    2. Meios com fio:
        1. Twisted Pair Cables
        2. Oaxial cables
        3. Fibra optico
    3. Sem fio:
        1. FIbra otica
        2. Ondas de radii
        3. Microondas
        4. Infravermelho

