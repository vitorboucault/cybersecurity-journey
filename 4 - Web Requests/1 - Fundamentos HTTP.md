# HTTP

A maioria das aplicações utilizam a internet e se comunicam através de requisições web através do protocolo HTTP.

A comunicação HTTP consiste em um cliente fazendo uma requisição ao servidor por um recurso, e servidor processa o request devolve o recurso.


## HTTPS

Protocolo onde todos os requests são transferidos em um formato encriptado, mesmo que um terceiro intercepte o request, ele não vai conseguir extrair os dados.

Mas, os requests ainda podem revelar a URL visita caso o servidor DNS seja contactado. Por essa razão é necessário utilizar servidores DNS encriptados como 8.8.8.8 ou 1.1.1.1, ou utilizar um serviço VPN, para garantir que o trafego seja encriptado apropriadamente.

## URL

Os recursos do HTTP são acessados via URL, que oferece varias formas de especificação do que simplesmente colando um site que queremos visitar.

![](*/imgs/url.png)

**Scheme** —> Usado para identificar o protocolo que o cliente está acessando

**User Info** —> Componente opcional para colocar credenciais, usado para autenticar o host
**Host** —> Pode ser o nome do host ou um endereço IP.

**Port** —> Separado do host com :, se nenhuma porta for especificada os schemes levam para a porta 80 ou 443

**Path** —> Aponta para um recurso especifico, pode ser uma pasta ou arquivo. Se nenhum caminho for especificado ele aponta para o default

**Query String** —> Começa com ?, e consiste em um parâmetro e valor. Múltiplos parâmetros podem ser separados por &

**Fragments** --≥ São processados pelo lado do cliente para localizar as seções com #

Nem todos os componentes são obrigatórios, os obrigatórios são o Scheme e o Host.


## HTTP FLOW

Os navegadores geralmente olha os registros na pasta /etc/hosts, se não existe, ai sim que eles contactam outros servidores DNS.

Assim que o navegador pega o endereço IP conectado ao domínio requisitado, ele envia um GET request para a porta padrão, pedindo pelo root/path. Ai, o servidor web recebe o request e processa ele.



## HTTPS FLOW

Dependendo das circunstâncias, um atacante pode performar um HTTP downgrade attack, que rebaixa o HTTPS para HTTP, fazendo com que os dados não sejam transferidos de forma encriptado. Isso pode ser feito via MITM proxy, transferindo todo o trafego para o host do atacante sem o conhecimento usuario. 