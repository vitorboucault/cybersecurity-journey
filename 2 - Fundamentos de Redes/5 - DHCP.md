# Dynamic Host Configuration Protocol (DHCP)

É um protocolo de gerenciamento de rede usado para automatizar o processos de configuração de dispositivos em redes IP.

Isso permite que os dispositivos recebam um endereço de IP automaticamente e outros parâmetros de configuração de rede, como:

1. Subnet mask
2. Default gateway
3. DNS Servers

Como funciona:

- Existe um servidor DHCP onde é um dispositivo, como um roteador, que mantem uma pool de endereços IP disponíveis

- E o DHCP client é o dispositivo que se conecta a rede e solicita as configurações do servidor DHCP

Esse processo se chama DORA (Discover, offer, request, acknowledge)

O IP que o dispositivo receber ele não é permanente, após 24h o dispositivo faz uma outra solicitação para continuar utilizando o IP.

Então o cliente manda uma DHCP discorre, após o a resposta, ele manda um DHCP Request para confirmar