# O problema da distribuição de keys

Como resolver o problema da criptogria simétrica onde não é possível compartilhar um key via rede?

## Criptografia assimétrica

Nesse tipo de criptografia se utiliza 2 tipos de key ao invés de 1.

- Uma key pública que todo mundo pode saber e usar
- Uma key privada que apenas 1 pessoa sabe e mantém segredo.

Se você criptografa algo com uma key publica de alguém, só a key privada dela pode descriptografar.

Se você criptografa algo com sua key privada, qualquer um com a key pública pode descriptografar.

As duas estão conectadas matematicamente, mas demoraria anos para recuperar a key privada a partir da pública.

## Resolvendo o problema da distribuição de keys

- Fulano cria a key publica e a privada no seu computador. Ele guarda a privada e compartilha a publica.
- Ciclano pega a key publica de Fulano
- Ciclano criptografa a mensagem de Fulano usando a key publica
- Fulano recebe a mensagem e descriptografa usando a key privada pessoal dele.

O HTTPS funciona dessa forma