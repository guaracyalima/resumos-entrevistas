# React

## Ciclo de vida
### Fases
- Inicialização
- Montagem
- Atualização
- Desmontagem

### Metodos de montagem

#### componentWillMount

- É executado quando o componente estiver prestes a ser montado no DOM da pagina
- Todas as ações a serem tomadas nesse estado devem ser definidas aqui
- É executado apenas uma vez no ciclo de vida do componente

#### Render

- Monta o componente no navegador
- É um metodo puro (função pura)
- Dá a mesma saida sempre que for fornecido a mesma entrada

####  componentDidMount

- É executadodepois que o componente for montado no DOM
- É eecutado apenas uma vez no ciclo de vida, sempre apos a primeira renderização
- Com ele podemos acessar o DOM, inicializar bibliotecas como JQuery, etc
- Chamadas a API's devem ser feitas neste ciclo

### Metodos de Atualização

A atualização começa quando o react já esta montado no navegador
- Componentes podem ser atualizados de duas maneiras:
via `props` ou atualizando seu estado

#### shouldComponentUpdate
- Informa ao react para que quando o componente receber nova props ou estado para re-renderizar ou
ignorar a rendereição.
- Mais usado quando a redenrização é um metodo muito pesado, logo deve ser evitado renderizar por completo, tendo sua renderização escalonada
- retorna sempre `true` ou `false`

#### componentWillUpdate
- É executado somente quando o metodo shouldComponentUpdate devolver `true`
- É usado apenas para preparar a proxima renderização
- É semelhante a um construtor

#### componentDidUpdate

- É excutado quando o novo compoente (já atualizado) foi atualizado na DOM
- É usado por exemplo para reativar bibliotecas de terceiros, garantindo que elas tabem recareguem (sejam 'atualizadas')

### Metodos que são chamados quando o compoente pai envia propos para os filhos

#### coponentWillReceiveProps
- É executado quando as props mudaram e não são mais processados pela primeira vez
- Se o estado depende da props, sempre que estas mudarem o estado tambem deve ser sincronizado


### Metodos de desmontagem

#### componentWillUnmount

- É o ultimo metodo no ciclo de vida
- É executado antes de  componente ser removido do DOM
- Um exemplo de uso seria o logut do usuario, remoção de tokens, etc
