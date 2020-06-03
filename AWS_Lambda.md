# AWS Lambda

- A função lamba pode ser utilizada como integrador dos serviços AWS para tanto ela apresenta algumas características

- Pode ser acionada através dos eventos gerados por outros serviços AWS

- Uma função Lambda pode servir de Trigger para outra função

- Obrigatoriamente devemos configurar um trigger para executar a função.

- prove uma maquina com configurações apropriadas, definidas pelo usuario

- Precisa-se definir uma quantidade de memoria que a função necessita para funcionar

- É preciso configurar um tempo maximo para a função, caso ela não seja concluida dentro desse tempo, a mesma é encerrada

- remove a obrigatoriedade de se realizar manutenções no servidor, sistema operacional, etc

- Basicamente não se tem um servidor, apenas serviços alocados para rodar a aplicação

- Pode se combinar o Lambda com outros recursos como S3, DynamoDB, etc para escalar a plicação

- Infraestrutura de alta disponibilidade
