# Conseguindo ajuda no Linux

Existem quatro formas de pedir ajuda no Linux:

- Comando exibe um manual -> `man <ferramenta>`

- Resumo rapido -> `<comando> —help`

- Resumo menor ainda -> `<ferramenta> -h`

- Comando que busca em todas as descrições dos manuais pela  palavra chave -> `apropos <palavra chave>

| Comando  | Quando usar  |
|---|---|
| `man ls`  | Quero entender tudo sobre o comando  |
|`ls --help`   | Quero ver as opções disponíveis rapidinho  |
| `curl -h`  | A ferramenta usa -h em vez de --help  |
| `apropos sudo`  | Não sei o nome do comando, só o que ele faz  |


O site [explainshell.com]() é um recurso valioso: você cola um comando longo e complexo, e ele explica cada parte separadamente com os trechos do próprio manual.

## O fluxo ideal de ajuda para pentesting

1. `-help  ou -h` -> visao geral rápida
2. `man` —> quando precisar detalhes específicos
3. Explainshell` —> quando encontrar um comando longo e complexo que nao entende