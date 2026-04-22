# STATUS CODES

São utilizados para informar o cliente do status da request dele. Um HTTP server pode retornar 5 classes de status codes:

- 1xx —> prove informação que nao afeta o processamento do request
- 2xx —> retorna quando um request foi bem sucedido
- 3xx —> retorna quando o servidor redireciona o cliente
- 4xx —> significa requests impróprios por parte do cliente.
- 5xx —> retorna quando existe um problema no servidor HTTP

Exemplos:

200 OK, 302 Found, 400 Bad Request, 403 Forbidden, 404 Not Found, 500 Internal Server Error