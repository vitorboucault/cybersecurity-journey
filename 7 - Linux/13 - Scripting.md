# Scripting e componentes

- `nano`: cria arquivo novo e edita

## Variaveis

- `read variavel`: serve para armazenar a variavel
- `chmod +x arquivo.txt`: da permissao pro script ser executado

## Loops

```
#Define o interpretador
#!/bin/bash
for i in {1..10};
do
echo $i
done
```

## Condicionais

```
#!/bin/bash
echo "Please enter your name first:"
read name
if [ "$name" = "Stewart" ]; then
echo "Welcome Stewart! Here is the secret: THM_Script"
else
echo "Sorry! You are not authorized to access the secret."
fi
```