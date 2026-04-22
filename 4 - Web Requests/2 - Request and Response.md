# HTTP REQUEST AND RESPONSES

Uma HTTP request é feita pelo client, e é processada pelo servidor. Assim que servidor recebe a request, ele processa e responde enviando uma HTTP response, que contem o código de response (response code).

## HTTP REQUEST

Method —> Especifica a ação
Path —> O caminho para o recurso ser acessado, também pode ser uma query string
Version —> É usada para denota a versão HTTP

As próximas linhas são para especificar vários atributos de uma request, os header terminam com uma linha nova, que é necessário para que o servidor valide a solicitação, e no final o request pode terminar com o body e data.

## HTTP RESPONSE

Contém a versão do HTTP e o response code do HTTP

Os response codes são usados para determinar status da request.

Após isso, o response lista o header, que é similar ao do HTTP request. E também tem no final o response body, que é definido como código HTML, mas também pode ser outros códigos como o JSON, recursos do website como imagens, tabelas ou scripts, ou até documentos.

## cURL

Ferramenta essencial para enviar vários tipos de web requests pela linha de comando.

Comandos

curl host ou endereço ip —> imprime html
curl -0 host ou endereço ip —> faz o download da página

Flag -k —> para pular a checagem do certificado SSL
Flag -v ou -vvv —> para ver de forma completa o HTTP request e response.
Flag -I —> envia um HEAD request e apenas exibe os response headers
Flag -i —> exibe os dois headers e o response body