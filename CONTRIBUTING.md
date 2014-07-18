# Contribuindo

## Introdução

Há várias maneiras de contribuir com o desenvolvimento do *Semantic*. Somos um projeto muito novo e estamos procurando grupos de entusiastas e pessoas que pensem da mesma forma que os colaboradores do *core* do Semantic. Usamos o livre e encantador software de gerenciamento de projeto [Trello](https://trello.com/jack148/recommend) para ficar atualizados com as questões do projeto.

Alguns quadros no Trello estão abertos ao público, outros são limitados aos colaboradores. Qualquer pessoa pode compartilhar idéias sobre o projeto usando nossos quadros públicos.

Se você quiser ser adicionado ao quadro de colaboradores do *Semantic* e estiver ativo na programação, por favor envie um e-mail (em inglês) ao autor [jack@myfav.es](mailto:jack@myfav.es)

### Publicidade

Uma das maneiras mais fáceis de manter o *Semantic UI* é disseminar o projeto mundo à fora.

## Fazendo um *Semantic* melhor

### *Bugs* & Problemas

Por favor, envie quaisquer *bugs* que você encontrar ao utilizar a biblioteca para o nosso [Rastreador de Problemas no Github](https://github.com/jlukic/Semantic-UI/issues?state=open).

Quando você reportar um *bug*, por favor inclua um conjunto de passos para reproduzir o problema e qualquer informação relacionada, *browser*, sistema operacional, etc. Caso contrário, não poderemos ver o problema, e isso tornará as coisas mais difíceis.

Por favor, crie uma cópia deste [jsfiddle](http://jsfiddle.net/pMDsH/) para demonstrar *bugs*.

### Guia de Estilo

Todos os colaboradores devem ler sobre as diretrizes de codificação do projeto. E o mais importante, ler o guia da linguagem, pois é uma das partes mais importantes partes do *Semantic UI*.

[Linguagem](http://br.semantic-ui.com/guide/styleguide.html)
[CSS](http://br.semantic-ui.com/guide/cssguide.html)
[Javascript](http://br.semantic-ui.com/guide/javascriptguide.html)

### *Pull Requests*

Qualquer pessoa pode decidir corrigir os bugs sozinhos, em *localhost*. Esta é provavelmente a melhor maneira de se tornar um colaborador do *Semantic*. Contudo, certifique-se de seguir as guias de estilo quando submeter o código.

*   [Solicite um Pull Request](https://github.com/jlukic/Semantic-UI/compare/)
*   [Veja Questões em aberto](https://github.com/jlukic/Semantic-UI/issues?state=open)

### Expansão UI

*Semantic* busca pessoas para ajudar a contribuir com novos componentes UI para o *core*, e sugerir extensões para a biblioteca.

Se você tiver sugestões de componentes que ainda não tem no *Semantic*, e gostaria de vê-los nas futuras versões, por favor adicione-os ao nosso Quadro Público de Componentes UI. A lista atual de futuros componentes e seu estado atual de desenvolvimento pode ser vista no quadro de Colaborador UI.

#### Visite os Quadros de Desenvolvimento UI

[Público](https://trello.com/b/Q8uTLy2T) |
[Colaboradores](https://trello.com/b/yVsh5Rds)

## Desenvolvimento das Especificações

Nós buscamos atualmente idéias sobre a melhor maneira de expandir o *Semantic*, para incluir nossa **biblioteca central** com **componentes de terceiros**. Isso requer a criação de uma especificação de componentes que possa ser utilizada por qualquer pessoa para criar componentes UI, e um sistema de gerenciamento de pacotes (site ou linha de comando) para que os autores possam distribuí-los.

Esses recursos são muito importantes para o crescimento saudável do ecossistema do *Semantic*, e para expandir o número de componentes disponíveis para os usuários.

#### Visite os Quadros de Desenvolvimento da Comunidade

[Público](https://trello.com/b/FZvMsVIM) |
[Colaboradores](https://trello.com/b/eOoZwNBQ)

---

## Desenvolvimento

Um guia para o desenvolvimento em servidor local.

## Running Locally

Pode ser útil executar a documentação de desenvolvimento em *localhost* quando se tem uma cópia/*fork* da versão do *Semantic*. Os próprios documentos ajudam a testar as alterações nos Componentes UI.

## Instalação no LINUX

### 1) Instalação do Node.JS

A documentação do *Semantic* é escrita em **DocPad** e requer o **Node.JS**.

Certifique-se de que o npm não precise de acesso sudo para funcionar, isso pode causar problemas de permissões.

*   [Node.JS via Package Manager](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager)
*   [Instalando Node.JS sem sudo](https://gist.github.com/isaacs/579814)

### 2) Instalando Dependências

```bash
npm install -g docpad
docpad install eco
docpad update; docpad upgrade
```

```bash
npm install -g grunt-cli
```

### 3) Dê um *Fork* no *Semantic*

[Fork](https://github.com/jlukic/Semantic-UI/fork)

### 4A) Construa o *Semantic*

Para ter a versão atual do *Semantic* disponível dentro de sua documentação local, você terá que construí-lo uma vez com **Grunt**.

```bash
grunt build
```

### 4B) Inicie o servidor

```bash
docpad run
```

**DocPad** agora deve executar uma instância do semantic-ui.com localmente.
Você pode acessar em `http://localhost:9778`

**Observe que alguns arquivos podem estar faltando até que você execute 'grunt build` uma vez.**

## Corrigindo *Bugs*

### Observe o Script

Se você está tentando corrigir um componente UI que faz parte do *Semantic*, a sua melhor aposta é a de trabalhar ativamente no arquivo em `/src/{tipo}/{nome do elemento}/` enquanto roda observa o script a partir do *grunt*. Isto irá reconstruir a documentação depois de fazer alterações, de modo que você possa ver se conseguiu corrigir o problema.

Para ver exatamente oque isso faz, você pode dar uma olhada no nosso [gruntfile comentado](https://github.com/jlukic/Semantic-UI/blob/master/Gruntfile.js)

```bash
grunt
```

A tarefa de observar o script é a tarefa padrão do *grunt* para o *Semantic*, assim você pode iniciar ele puro e simples.

### Empacotanto elementos

Por conveniência, existe também um comando *grunt* separado para construir *minified* (minificadas), *packages* (pacotes), e *compressed* (compactadas) versões da biblioteca.

```bash
grunt build
```


## Instalação no WINDOWS

> em breve

## O Futuro

### UI Dev Kits

Estamos trabalhando para criar kits de desenvolvimento para escrever e distribuir definições UI de terceiros. Estes, são planos para o projeto depois da nossa versão 1.0 que permitem que outros desenvolvedores contribuam com componentes UI ou redesign de componentes existentes.

Para mais informações sobre o desenvolvimento da especificação UI para componentes de terceiros, por favor, visite os nossos quadros de discussão da comunidade no Trello

#### Quadros de Desenvolvimento
[Público](https://trello.com/b/FZvMsVIM) |
[Colaboradores](https://trello.com/b/eOoZwNBQ)
