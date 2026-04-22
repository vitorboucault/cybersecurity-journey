# DNS

Fornece uma forma simples para a gente se comunicar com os dispositivos na internet, sem precisar ficar lembrando de numeros complexos.

## Hierarquia de Dominios

### TLD (Top-Level Domain)

É parte mais a direita dos dominios, exemplo:

- .com
- .online
- .club

Serve para representar o proposito do dominio.

### Second-Level Domain

É a parte de "texto" do dominio, por exemplo:

**hackthebox.com**

- hackthebox é Second-Level Domain
- .com é o TLD

### Subdomain

Fica no lado esquerdo do Sub-Level domain, por exemplo

- admin.hackthebox.com
  - admin nesse caso é o subdominio

## DNS Record Types

### A Record

Utilizado para endereços IPV4.

### AAAA Record

Utilizado para endereços IPV6

### CNAME Record

Registros que apontam para outro nome de dominio.

Exemplo: eu tenho um dominio loja.vitorboucault.com, quando eu entro nele, abre uma nova guia e aponta pra outro dominio que eu determino.

### MX Record

Apontam para o servidor de email do dominio requisitado.

### TXT Record

São campos de texto livre onde quase dado de texto pode ser armazenado.

## O que acontece ao fazer uma DNS Request?

1. O computador confere o cache local para ver se o endereço não foi acessado recentemente, se não, um recursive DNS Server vai ser feito.
2. Geralmente a nossa ISP fornece esse servidor DNS recursivo, mas pode ser escolhido de forma própria também. Se encontrado localmente, o resultado é enviado para a maquina, se não começa a jornada para encontrar a resposta correta.
3. O root serve atua como a dorsal do DNS n internet, seu trabalho é nos redicionar para o TLD correto.
4. O servidor TLD guarda os records para encontrar onde achar o server autentico (nameserver) para responder a DNS request.
5. O nameserver/authoritative é responsável por guardar os DNS records