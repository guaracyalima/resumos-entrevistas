# REDUX
### Definição
`É um container de estados previsvel para aplicações JavaScript, inspirado na arquitetura flux e Elm - linguagem funcional que compila para javascript`

#### Estrutura

##### Actions

`Descrições de como o estado será modificado`

- Contem um type (string)
- Contem um Payload (valor da action)

Actions são objects

##### Reduces

`São funções puras que recebem o estado atual, a action e retornam o estado modificado de acordo com a action`
- nunca devem mudar o estado, retornando sempre uma copia do estado quando o mesmo for alterado

##### Store

- Aplicações redux possuem uma única store

`ìmport { createStore } from 'redux'`

`const store createStore(reducer)`

- cada store recebe um unico reducer
- Exite o metodo de combine reducer

Possui apenas 3 metodos:

- Dispatch => Comunica actions para a store

- getState => Consulta o estado da aplicação, retorna o estado completo

- subscribe => registra um callback que é executado sempre que um novo estado é gerado apartir de uma action

- Redux não suporta actions assincronas

### Middlewares

- Usadas para converter actions assincronas em sincronas

- É uma função que transforma as actions antes de passlas para os reducers da aplicação

um dos bem conhecidos é o redux-thunk. Permite que você lance uma fnção que aceita o metodo getState e outro Dispatch e executa a função antes que ela chegue no reducer
