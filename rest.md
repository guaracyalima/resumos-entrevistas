
# SOFEA  - Software Oriented Front End Architecture
Arquitetura de front end orienteada a serviços


## Modelo de maturidade de Richardson

## Level 0

- não é REST
- http apenas como transporte

## Level 1
- ainda não é rest
- adiciona a visão de recurso
- não faz bom uso do protocolo http

## Level 2
- é REST
- Faz uso dos verbos HTTP e seus codigos de retorno
- Retorna um location com a representação do recurso

## Level 3

- REST Full
- cabeçalhos de resposta
- Faz uso dos verbos HTTP e seus codigos de retorno
- Mais acoplado ao protocolo HTTP
- Retorna um location com a representação do recurso


## HATEOAS
- Hypertext As The Engine Of Application State
- São links de ações de como iteragir com o recurso

## Idempotencia
- Um metodo é considerado idempotente se o resultado por ele produzido é sempre o mesmo, independente do número de vezes em que é executado
