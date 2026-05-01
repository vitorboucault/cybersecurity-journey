# Permissões

Um arquivo ou diretório pode conter várias informações e também tipos de usuários com diferentes tipos de permissões, que são:

- Ler `(Read)`
- Escrever `(Write)`
- Executar `(Execute)`

## Diferenças entre Usuários e Grupos

### Trocando entre usuários

- Comando `su`

Para trocar é necessário saber qual usuário iremos trocar e é necessário saber a senha dele.

## Entendendo permissões de arquivos em Formato Numérico

As permissões geralmente são mostradas em formato simbolico como

`rwxrwxrwx`

- `r` = read
- `w` = write
- `x` = execute

## Convertendo Permissões Simbólicas em Números

- Read (`r`) tem valor 4
- Write(`w`) tem valor 2
- Execute(`x`) tem valor 1

| Simbolico    | Numerico | Significado                                                 |
|--------------|----------|-------------------------------------------------------------|
| `rwxr-xr-x`  | 755      | Root pode fazer qualquer coisa, outros podem ler e executar |
| `rw-r--r--`  | 644      | Root pode ler/escrever e os outros podem apenas ler         |
| `rwx-------` | 700      | Apenas o root tem acesso                                    |

## Por que isso é importante?

- Vários comandos linux usam valores numeros (ex.: `chmod 755 file`)
- Você identificar rapidamente riscos de segurança
- Voce pode controlar quem acessa arquivos sensiveis
