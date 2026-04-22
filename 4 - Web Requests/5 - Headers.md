# HTTP Headers

Os headers podem ter 1 ou múltiplos valores, e eles podem ser divididos em:

- **General Headers:**

    - São contextuais e usados para descreve a mensagem em vez de seu conteúdo
    - Pode ser usado no request e no response
    - Contém data e e conexão (date and connection)

- **Entity Headers**

    - Pode ser usado no request e no response
    - Usados para descrever o conteúdo, utilizado em responses de POST ou PUT requests
    - Contém: content-type: text/html, media-type: pdf, boundary="1212”, content-length: 385, content-encoding: zip

- **Request Headers**

    - São usados no HTTP request e não tem relação com o conteúdo da mensagem
    - Contém o host, user-agent, referee, accept, cookie, authorization.

- **Response Headers**

    - Pode ser usado em um HTTP response e não é relacionado com o conteúdo.
    - Contém: server, set-cookie, WWW-authenticate

- **Security Headers**

    - É uma classe de response readers usados para especificar algumas regras e politicas a serem seguidas pelo browser enquanto acessa um website
    - Contém content-security-policy, strict-transport-security, referrer-policy

## Headers comuns de Request

- Host: fala qual website está sendo requisitado
- User-Agent: informa o tipo e a versao do browser
- Content-Length: tamanho do conteudo
- Accept-Enconding
- Cookie: sao salvos para relembrar ao navegador quem voce é

## Headers comuns de Response

- Set-Cookie
- Cache-Control
- Content-Type: fala pro browser o tipo do conteudo
- Content-Enconding

Existem outros tipos de HTTP Headers, mas esses 5 acima são os mais comuns.
