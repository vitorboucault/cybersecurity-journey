# Segurança de Rede

O termo segurança remete a medidas que protegem dados, aplicações, dispositivos, e sistemas em uma rede de acesso não autorizado.

A meta é manter a trindade CIA:

1. Confiabilidade
2. Integridade
3. Acessibilidade

## Firewalls

É um dispositivo de segurança de rede, que monitora a entrada e saída do trafego de rede. Ele coloca uma série de regras conhecida como firewall policies ou Access control Lists.

Opera analisando os pacotes de dados, de acordo com regras e politicas predefinidas, focando em fatores como endereço IP, números de portas e protocolos.

Tipos de firewall:

1. Packet Filtering Firewall
    1. Opera nas camadas 3 (Network) e 4 (Transport) do modelo OSI
    2. Examina a fonte e destino do ip e porta e o tipo do protocolo.
2. Stateful Inspection Firewall
    1. Localiza o estado das conexões de rede
3. Application Layer Firewall (Proxy Firewall)
    1. Opera na camada 7 (aplicação) do modelo OSI
    2. Inspeciona o conteúdo atual do tráfego e bloquei solicitações maliciosas
4. Next-Generation Firewall (NGFW)
    1. Inspeção profunda de pacotes, detecção/prevenção de intrusões e controle de aplicativos
    2. Implemente recursos avançados como DPI, deep packet inspect

Os firewall ficam entre a internet e nossa rede interna, protegendo e analisando o tráfego, antes de ser passado.

## Intrusion Detection and Prevention Systems (IDS/IPS)

São soluções desenvolvidas para monitorar e responder a atividades suspeitas na rede.

Um IDS observa trafego e sistemas de eventos para identificar comportamento malicioso ou violação de politicas, gerando alertas mas não bloqueando o trafego suspeito.

Um IPS detecta, e previna bloqueando trafego suspeito de rede.

Técnicas:

1. Signature-based detection:
    1. Compara o tráfego com um banco de dados de exploits conhecidos
2. Anomaly-based detection:
    1. Detecta qualquer coisa fora do usual comparado com a atividade normal