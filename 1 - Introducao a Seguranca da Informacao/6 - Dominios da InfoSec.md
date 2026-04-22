# Dominios da InfoSec

## Segurança de Rede

A segurança de rede é um componente crucial para a infosec, que protege a rede e os dados transmitidos através dela. Utiliza ferramentas como:

1. Firewall:  atua como uma barreira entre redes internas confiáveis e redes externas não confiáveis, filtrando o tráfego baseado em regras de segurança preestabelecidas
2. IDS/IPS: Monitora o tráfego de rede para encontrar atividades suspeitas e tomar decisões automatizadas para detectar e bloquear possíveis ameaças
3. VPNs: Provê segurança, conexão encriptada sobre as redes públicas, garantindo a privacidade e integridade dos dados.
4. Mecanismos de controle de acesso: Inclui autenticação: protocolos de autorização e autenticação que garante que apenas usuários legítimos acessem os recursos de rede
5. Tecnologias criptografadas: protege dados sensíveis em trânsito ou parados, fazendo com que seja impossível de ler para partes não autorizadas

Responsabilidades do time segurança de rede

O time de segurança de rede é responsável por desenvolver, implementar e manter a infra da segurança de rede de uma empresa. Isso inclui configurar e gerenciar a segurança dos dispositivos, desenvolvendo e reforçando as políticas de segurança, monitora tráfego e ameaças em potencial respondendo a incidentes de segurança.

Testar a segurança de rede é um aspecto crítico para manter a sua efetividade.


## Segurança de Aplicativos

A segurança de aplicativos é um componente critico da segurança da informação e é um fator significante em brechas quando não implementado da maneira correta.

A meta principal é garantir que os aplicativos são desenvolvidos, implantados e mantidos de uma maneira que preserve a trindade CIA dos dados que eles processam e sistemas que eles interagem.

Isso é crucial pro cenário atual pois os aplicativos lidam com dados e informações sensíveis e estão sujeitos a uma seria de potenciais ameaças de agentes maliciosos

A Segurança de Aplicativos começa nos estágios iniciais do ciclo de desenvolvimento de software e continua ao longo da implementação e manutenção.

Envolve uma combinação de praticas de código seguros, testes de procedimentos rigorosos e a implementação de vários controles de segurança.

Os deve precisam escrever códigos que aderem as melhores praticas de segurança e resistência a vulnerabilidades como SQL injection, crosssite scripting (XSS) e overflow de buffers.

Responsabilidade da Segurança de Aplicativos

Os devs de aplicativos estão na linha de frente, responsáveis por escrever códigos seguro e implementar recursos de segurança.


Arquitetos de segurança são responsáveis por projetar a estrutura geral de segurança das aplicações e sua infra de suporte.

Os times de operações de TI são responsáveis por fazer a gestão da segurança dos ambientes de produção onde as aplicações vão rodar.

O Gerente de Segurança de Aplicativos é responsável pela gestão geral da segurança de apps, ou em operações maior é o CISO. Eles são responsáveis por setar a politicas de segurança dos apps, garantindo conformidade com os padrões de segurança e regulações, revisando a implementação das medidas de segurança em toda a organização.

Os pen. testers ou os security testers fazem os testes de segurança nos aplicativos.

## Segurança Operacional

Pode ser abreviado como OpSec. É crucial para a estratégia de segurança geral da organização. Isso abrange processos, práticas e decisões relacionada a lidar e proteger os ativos de dados durante todo o ciclo de vida.

A meta principal da OpSec é manter um ambiente seguro para o dia a dia operacional da organização, garantindo que os dados sensíveis continuem sendo confidenciais, intactos e disponíveis apenas para as pessoas que são autorizadas.

1. Identificação de ativos
    1. A organização precisa identificar dados sensíveis que precisam de proteção especial
2. Identificação de ameaças
    1. A organização precisa analisar as ameaças e ver onde as coisas podem dar errado.
3. Identificação de ameaças
    1. Envolve implementar medidas de segurança como senhas, crachás de segurança, e até câmeras de segurança para proteger informações importantes
4. Controle de acesso
    1. A equipe de OpSec determina quem pode acessar dados sensíveis, garantindo que apenas as pessoas certas tenha as permissões necessárias.
5. Monitoramento
    1. A equipe de OpSec precisa monitorar tudo em um processo continuo para adaptar-se a novas ameaças e mudança para manter tudo seguro

### Responsabilidades da OpSec

A OpSec precisa trabalhar junto com outros departamentos como o de TI, Recursos Humanos e o departamento jurídico, para garantir que as medidas de segurança estão alinhadas com a necessidade do negocio e requisitos regulamentares.

É necessário comprometimento e cooperação de todos os níveis da organização, dos colaboradores da linha de frente até os executivos do alto escalão.

## Recuperação de desastres e continuidade de negócios

São componentes importantes da estratégia de resiliência de uma organização. Esses dois conceitos precisam ter focos e metodologias distintas. Lida com a restauração de eventos críticos.

Eventos como desastres naturais como terremotos ou enchentes, desastres feitos pelo homem como incêndios ou terrorismo, ou falhas na tecnologia como travamento de sistemas ou ciberataques.

O foco é minimizar o tempo parado e a perda de dados. O plano da DR inclui procedimentos detalhados de backup de dados, replicar sistemas e utilizar o método failover para alternar sites ou ambientes de cloud.

DR (Disaster Recovery) 
Foca em restaurar as partes criticas do sistema e de dados depois de algo ruim acontecer. A essência é juntar as peças novamente e botar para as coisas voltaram a funcionar o mais rápido possível.

BC (Business Continuity)

Paras as empresas, BC significa descobrir como manter operações durante e depois de uma  interrupção. Envolve os trabalhadores dando turnos em casa, utilizando fornecedores alternativos ou até se mudando para um escritório temporário.

Um bom time de DR/BC pode ser a diferença entre uma empresa enfrentando crise ou sucumbindo a ela. E não apenas para proteger contra perdas financeiras, mas ajuda a manter a confiança do consumidor, manter os requisitos regulatórios e proteger a imagem da empresa

Responsabilidade

Eles são responsáveis por desenvolver, implementar e manter os planos de DC/BC junto com o time de TI. Eles fazem avaliações de risco, identificam funções criticas no negócio, criam objetivos de tempo de recuperação (RTO) e objetivos de ponto de recuperação.

## Segurança de Cloud

A segurança de cloud serve para manter os dados e aplicações seguras quando armazenadas em cloud.

Áreas que a segurança de cloud protege

- Proteção de dados: encriptação de dados quando guardados e em transito.
- Gestão de Identidade e Acesso (IAM): Senha personalizada ou código de acesso para pessoas autorizadas
- Network Security: Firewall e VPS que protege o dado enquanto ele é movimentado pela rede
- Compliance e Governança envolve seguir as leis e regulações sobre como os dados devem ser assegurados e manuseados, garantindo que o que for feito tenha conformidade com os padrões legais e legais da industria

### Responsabilidade

A responsabilidade da segurança é dividida em: 
- Provedores de segurança
- Você (Eu)
- Times de segurança

Mudar proteções antigas e atualizar as medidas de segurança regularmente.

## Segurança fisica

Tem como meta de proteger fisicamente que pessoas não autorizadas acessem recursos importante, que podem levar a brechas nos dados, roubo e até danos.

A meta principal é criar camadas de proteção para deter, detectar, atrasar e responder a possíveis ameaças que são físicas.

É importante porque: 
- Protege ativos valiosos, equipamentos caros e dados críticos em dispositivos físicos.
- Protege o pessoal, garantindo que os colaboradores tenham e visitantes estejam seguros.
- Ajuda a manter a operação funcionando e prevenindo de interrupções causadas por brechas de segurança
- Faz parte do compliance que regula as empresas, então muitas industrias precisam implementar medidas físicas de segurança especificas que protegem os dados sensíveis

Responsabilidades

Recai sobre o uma equipe ou o departamento de segurança física dedicado. Geralmente, esse time se reporta ao CSO ou CISO em empresas que as informações físicas e digitais são integradas.

A segurança fisica também envolve outros cargos:

- Equipe que faz a gestão das instalações da organização
- Time de segurança da TI
- Todos os empregados são responsáveis por seguir os protocolos de segurança

Existem vulnerabilidades físicas como:

- Pontos de acesso inseguros como janelas, portas ou outro ponto de entrada
- Cadeados fracos, quebrados
- Perimetro de segurança inadequado
- Gestão das chaves
- Falta de luz, luz baixa
- Infra de TI exposta
- Gestão das visitas
- Workstations não supervisionadas

Até as medidas de cibersegurança mais sofisticadas podem ser inefetivos se o atacante ganhar acesso fisico

## Segurança Mobile

O principal objetivo da segurança mobile é proteger informações que são armazenadas ou transmitidas.

Camadas da proteção mobile:

1. Segurança de dispositivos
2. Segurança de dados
3. Segurança de rede
4. Segurança de aplicativos

## Internet of Things Security 

IOT Security é como se colocássemos cadeados, alarmes e seguranças aos apetrechos digitais, protegendo nossa casa de estranhos.

Os dispositivos IOT possuem poder de processamento e memória limitados, o que torna a implementação de segurança mais difícil sem afetar a performance.

Responsabilidades

- Liderados por um CISO ou um gerente de segurança de IoT.
- Proteger um ecossistema IoT é uma responsabilidade compartilhada que envolve pontos importantes:
    - Desenvolvedores dos dispositivos precisam faze-los já pensando na segurança desde o inicio. Isso inclui seguir princípios de design, minimizando recursos desnecessários que podem ter vulnerabilidades.
    - Administradores de rede protegem a rede que os dispositivos estão conectados.
    - Desenvolvedores de aplicativos implementam métodos apropriados de educação, para que apenas usuários confiáveis possam acessar os aplicativos.