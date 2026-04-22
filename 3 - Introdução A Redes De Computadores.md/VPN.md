## VPN

É uma tecnologoia que permite que dispositivos em redes separadas para se comunicar de forma segura, criando um caminho dedicado entre eles pela internet (isso é conhecido com tunnel)

Dispositivos conectado no tunel forma sua propria rede privada.

Existem vários tipos de VPN (Virtual Private Network), porém todos tem o mesmo objetivo:

### PPP (Point-To-Point Protocolo)

Tecnologia usada pela PPTP. Esse protocolo estabele uma conexão direta entre dois nós. Mas não oferece criptografia

### PPTP (Point-To-Point Tunneling Protocol)

Tecnologia que permite que o dado do protocolo PPP viaje e deixe e a rede.

### IPSec

Internet Protocol Security utiliza o framework IP na criptografia de dados.

Dificil de configurar mas pode dar um boost na criptografia dos dados.

### Site-To-Site VPN

Cliente e servidor são dispositivos de rede, geralmente roteadores ou firewall, e compartilha um intervalo inteiro de rede.

### Remote Access VPN

Envolve a criação de uma interface virtual no computador do cliente que se comparta como se estivesse na rede do cliente. Um aspecto importante ao analisar essas VPNs é a tabela de roteamento criada ao conectar-se a VPN.

Se o VPN cria uma rota especifica para a rede, ela é chamada de Split-Tunnel VPN, significando que a conexão de internet não sai da VPN.

Isso para uma empresa não é ideal, por que se a maquina estiver infectada por um malware, métodos de detectação em rede não vão funcionar, uma vez que o tráfego é encaminhado para a internet.

### SSL VPN

VPN que funciona em um web browser