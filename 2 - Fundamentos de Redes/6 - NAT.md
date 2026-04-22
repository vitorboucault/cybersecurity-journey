# Network Address Translation (NAT)

O NAT permite que múltiplos dispositivos em uma rede privada compartilhem do mesmo endereço de IP público

Endereços de IP privado, ajudam a conservar os IPs públicos.

É um processo realizado por um roteador ou dispositivo semelhante, que modifica o endereço IP de origem ou de destino nos headers dos pacotes IP, a medida que eles vão passando por eles.

Essa modificação é usada para traduzir o endereço privado de dispositivos em uma rede local para um IP publico.

## Tipos de NAT:

1. NAT Static:
    1. Mapeamento 1 a 1:
    2. onde cada endereço privado corresponde diretamente a um endereço de IP publico.
2. NAT Dinâmico:
    1. Atribui um IP público de uma pool de endereços disponíveis a um endereço de IP privado conforme a demanda da rede.
3. Port Address Translation (PAT):
    1. Múltiplos endereços de IP privado dividem um endereço de IP publico diferenciando as conexões usando os números de portas.
    2. Muito usado em casa e pequenos escritórios.

## Benefícios:

1. Guarda os endereços IPV4 limitados
2. Fornece uma camada básica de segurança não expondo diretamente a estrutura de rede
3. Flexível para o esquema de endereçamento de IP interno

## Trocas:

1. Serviços complexos como um servidor publico que utilizam o NAT precisam de configuração adicional
2. NAT