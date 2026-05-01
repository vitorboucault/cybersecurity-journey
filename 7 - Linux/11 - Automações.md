# Automações

- `cron` é o comando para automatizar tarefas no Linux
- `crontab` é o processo que inicia durante o boot, que é responsável por facilitar e gerenciar os jobs do `cron`.

Crontab precisa de 6 valores:

- `MIN`: Qual minuto executar
- `HOUR`: Qual hora executar
- `DOM`: Qual dia do mês executar
- `MON`: Qual mês do ano executar
- `DOW`: Qual dia da semana executar
- `CMD`: O comando que vai ser executado

Existe o [CronTab Generator](https://crontab-generator.org/) para gerar o formato necessário para colocar a data correta do comando

- `crontab -e` serve para editar o crontab


