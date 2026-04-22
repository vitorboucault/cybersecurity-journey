# Comunicação de rede

Existem 3 componentes cruciais para a rede funcionar e facilitar a comunicação, existem 3 componentes essenciais: 
1. **Endereços MAC:**
    1. É um identificador unico atribuído ao NIC de um dispositivo, permitindo que ele seja reconhecido em uma rede local.
    2. Opera na layer 2 do modelo OSI
    3. Eles tem 48 bits de comprimento, os primeiros 24 representam o OUI e os outros restantes são específicos para o dispositivo individualmente.
    4. São usados para comunicação local nas LANs
    5. O ARP é responsável por mapear os endereços IP para os endereços MAC. Permitindo que os dispositivos encontrem o endereço MAC pelo IP na mesma rede.
2. **Endereços IP:**
    1. É um numero atrelado a cada dispositivo conectado a uma rede que utiliza o Internet Protocol para comunicação.
    2. Funciona na layer 3 do modelo OSI
    3. Existem duas versões: ipv4 e ipv6
    4. Roteadores utilizam os endereços IP para determinar o caminho ideal para que o dado chegue ao destino
    5. Os endereços IP são flexíveis diferente do endereço MAC
3. **Portas**
    1. É o numero de um processo associado a um processo ou serviço em uma rede.
    2. Funciona na layer 4
    3. Facilitam a operação simultanea de vários serviços de rede em um mesmo endereço IP, diferenciando o trafego destinado a diferentes aplicações
    4. As portas variam de 0 a 65535 e são divididas em 3 categorias:
        1. **Well-Known Ports (0-1023):**
            1. Reservadas para servicos e protocolos comuns e universais padronizados e gerenciados pela IANA
            2. FTP utiliza a porta 20 e 21
        2. **Registered Ports (1024-49151):**
            1. São portas usadas para serviços externos que os usuários podem instalar no dispositivo.
            2. Tipo o Microsoft SQL server na porta 1433
        3. **Dynamic/Private Port (49152-65535)**
            1. Portas efêmeras, usadas para client Applications para enviar e receber dados dos servidores.
            2. Não são portas fixas

