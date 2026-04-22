# Arquitetura de Internet

Descreve como o dado vai ser transmitido, organizado e gerenciado pela rede.

## Peer-To-Peer (P2P)

Cada node atua como cliente e servidor

As redes P2P podem ser totalmente descentralizadas.

Tem como vantagem a escalabilidade, resiliência e distribuição de custo.

E tem como desvantagem a complexidade do gerenciamento, problemas de confiabilidade e desafios na segurança devido a exposição dos nomes.

## Cliente-Server Architecture

Uma das arquiteturas mais usadas da internet.

Nesse setup, o cliente manda requests e o servidor responde a esses requests.

Quando pesquisamos algo, um site por exemplo, fazemos um request para o site, e o servidor que armazena os dados do website e lida com os requests, recebe a query e processa localizando a pagina requisitada e envia de volta o dado para o browser, que recebe a informação e mostra a webpage.

O componentes chave dessa arquitetura é o tier model, que organiza o papel do servidor em camadas.

1. Single-Tier Architecture:
    1. O client, server e a database ficam na mesma maquina
    2. Setup raramente usado em aplicações de larga escala devido a limitações na escalabilidade e segurança
2. Two-Tier Architecture:
    1. Divide o ambiente da aplicação em client e servidor.
    2. O cliente lida com a camada de apresentação e o servidor com a camada de dados
    3. Esse modelo é visto em aplicações desktop, onde a interface está na maquina do usuário e o database no servidor.
3. Three-Tier Architecture:
    1. Introduz um camada adicional entre o cliente e o database do servidor, conhecida como application server.
    2. O application server lida toda parte logica e de processamento do negocio.
    3. Essa separação fornece flexibilidade e escalabilidade por que cada camada é desenvolvida e mantida de forma independente
4. N-Tier Architecture
    1. Usado em sistemas complexos
    2. N significa a quantidade de tiers separados entre três.
    3. Envolve multiplas camadas de servidores aplicação
    4. Altamente escaláveis
    5. Ideal para aplicações web e serviços que demandam robustez e soluções flexíveis
    6. Apesar de promover melhoras, eles também são introduzidos a complexidade na implantação e manutenção

## Hybrid Architecture

Mistura elements do Client-Server e Peer-To-Peer. Servidores centrais são usados para facilitar a coordenação e autenticação de tarefas. Essa combinação aproveita a força das duas arquiteturas para melhorar a eficiência e performance.

Aumenta a eficiencia e o controle, porém a implementação é complexa e existe um potencia me falhar em pontos específicos

## Cloud Architecture

Essa arquitetura opera numa escala virtualizada seguindo o modelo cliente-servidor. Fornece acesso a recursos por demanda pela internet. Serviços como Google Drive ou Dropbox são arquiteturas em Cloud, e são SaaS.

Cinco características que definem a arquitetura Cloud:

1. Serviço por demanda
2. Amplo acesso a rede
3. Compartilhamento de recursos
4. Elasticidade rápida
5. Serviço por uso

Como vantagens tem a escalabilidade, custo e manutenção reduzidos e flexibilidade. Por outro lado, existe dependência de um vendedor/serviço, problemas de segurança e conformidade e conectividade que demanda acesso a internet estável para acessar os recursos.

## Software-Defined Architecture (SDN)

Abordagem moderna de rede que separa o plano de controle, que toma as decisões de onde o trafego vai ser enviado, para o plano de dados, que encaminha o tráfego.

Promete um ambiente de gerenciamento de rede programável, permitindo assim, que os admins ajustem dinamicamente as politicas de rede e roteamento quando necessário.

Grandes empresas usam para alocar o tamanho de banda e gerenciar o fluxo de trafego de acordo com a demanda em tempo real.

A vantagem é que simplifica o gerenciamento de rede, as configurações podem ser feitas rapidamente por meio de softwares e é possível otimizar o fluxo de trafego dinamicamente, melhorando a utilização dos recursos.

As desvantagens é que se o controle central cair a rede pode ser afetada negativamente e exige novos conhecimento técnicos e softwares/hardwares especializados.