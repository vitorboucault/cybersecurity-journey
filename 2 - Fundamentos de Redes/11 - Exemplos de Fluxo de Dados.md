# Exemplo de Fluxo De Dados

1. **Acesso a internet**
    1. Primeiro o notebook identifica a rede sem fio correta/SSID
    2. Se a rede usa WPA2/WPA3, o usuário precisa fornecer a senha correta para autenticar
    3. Depois a conexão é estabelecida e o protocolo DHCP toma conta para configurar o IP
2. **Checando Configuração de Rede Local**
    1. Ao tentar acessar um website, o browser se prepara para enviar um request para a página
    2. Antes do pacote sair do notebook, o sistema checa se o IP é valido para a area da rede local
    3. Endereçamento de endereço de IP, caso o laptop ainda não tenha um.
    4. O DHCP endereço um IP privado ao laptop
3. **Resolução DNS**
    1. DNS Query, o laptop envia uma DNS query ao DNS Server
    2. O servidor DNS olha pro dominio e retorna o endereço de IP
4. **Encapsulamento de Dados e Local Network Transmission**
    1. Agora que o notebook tem um IP, começa a preparação para a transmissão de dados
    2. Os próximos passo ocorrem de acordo com o modelo OSI/TCP-IP:
        1. Camada de aplicação, o browser cria um HTTP request para a pagina
        2. Transport Layer, a solicitação está dentro de um segmento TCP  (ou UDP) e o segmento inclui fonte e portas de destino
        3. Internet Layer, o segmento TCP é colocado no pacote IP.
        4. Link Layer, o pacote IP é finalmente colocado no Frame ethernet ou wi-fi Frame. Aqui, o os endereços MAC são incluídos
5. **Network Address Translation (NAT)**
    1. Quando o roteador recebe o Frame, ele processa o pacote IP. Nesse ponto, ele faz a troca do ip privado para o ip publico. Nesse processo, o pacote passa por varios roteadores intermediários que vão encontrar o melhor caminho para alcançar a rede
6. **Servidor recebe o request e responde**
    1. Chegando na rede de destino, o firewall verifica se o trafego na porta 80 ou 443 é permitido
    2. Se passa da regra do firewall, ele vai pro host do server.
    3. Depois, o software do web server recebe e processa o request e prepara a webpage e envia de volta como uma resposta.
    4. O processo de resposta do servidor é o caminho reverso.
7. **Desencapsulamento e exibição**
    1. O laptop recebe a resposta e remove o Ethernet/Wi-fi Frame, o header IP e o header TCP, até a camada de dados da aplicação ser extraída.
    2. O browser lê o HTML/CSS/JavaScript e mostra a página