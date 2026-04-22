# Outros componentes

## Balanceador de carga

Um site com um load balancer, quando você faz uma requisição, ele vai procurar os servidores que estão disponíveis para responder a sua requisição

Caso um servidor não responda, o load balancer vai parar de enviar trafego para aquele servidor até que ele volte ao normal, isso se chama **health check**

## CDN (Content Delivery Networks)

Serve para cortar boa parte do trafego de um site ocupado.

Ele permite que você armazene ativos do seu site, em servidores de todo o mundo, e quando alguem faz uma requisição pra esse ativo, o algoritmo vai buscar no servidor mais proximo da pessoa.

## Databases

Servidores Web podem se comunicar com bancos de dados para armazenar e chamar informações e dados através deles.

## WAF (Web Application Firewall)

Fica localizado entre a web request e o servidor, ele funciona como uma barreira que analisa o trafego enviado para o servidor, se os requests passarem do "comum" ele não envia o request para o servidor

