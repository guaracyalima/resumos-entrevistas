# EJB - Enterprise Java Beans

Definição:

- É um pedaço de codigo java que executa em um ambiente de tempo de execução especializado
  chamado container EJB, o qual fornece um numero de componentes e serviços. Os serviços de persistência são fornecidos por um framework provedor especializado chamado de `provedor de persistência`

- São objetos java regulares que podem ser configurados usando anotações de metadados

### Caracteristicas

- Beans podem ser reutilizaveis
-

### Tipos de EJB

#### `Beans de seção`

- Usados para implementar a logica corporativa de uma aplicação EJB

- É excutado por um cliente afim de realizar alguma operação de negocio especifica

- O nome `seção` se deve ao fato de o bean está disponivel durante a duração de uma "unidade de trabalho", não sobrevivendo assim à uma queda do servidor ou a paradas temporarias

- Pode modelar qualquer regra de negocio da aplicação

- Se possuir estado, salva a seção do bean entre as invocações sem a neceidade de escrever codigo adicional

- Se não possuem estado, consequentemente não guardam qualquer estado

- Pode ser executado localmente quanto remotamente usando RMI

- Se não possuir estado pode ser exposto como sendo um WebService

#### `Beans dirigidos por mensagem`

- Usados para implementar a logica corporativa de uma aplicação EJB

- Processam regras de egocios

- Nunca são executados diretamente por clientes

- São invocados por mensagens enviadas pelo servidor de mensagens, o qual permite o envio de mensagens assincronas entre os componentes.

- São usados para integraçao robusta de sistemas ou para processamento assincrono

#### `Entidades`

São mais comunmente usados para implementar a persistência

### Serviços do EJB

- Transações
- Segurança
- Persistência
- Chamadas remotas
- Interceptadores
- Timers
- Gerenciamento de estados
- Envio de mensagens
