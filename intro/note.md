# </> htmx

    "High power tools for HTML"
    https://htmx.org/docs/

## 00. Intro:

htmx gives you access to AJAX, CSS Transitions, WebSockets and Server Sent Events directly in HTML, using attributes, so you can build modern user interfaces with the simplicity and power of hypertext

htmx is small (~14k min.gz’d), dependency-free, extendable & has reduced code base sizes by 67% when compared with react

## Reference:

### htmx Core Attributes

| Atributo        | Descrição                                                                 |
|-----------------|---------------------------------------------------------------------------|
| hx-get          | Emite uma solicitação GET para a URL especificada                         |
| hx-post         | Emite uma solicitação POST para a URL especificada                        |
| hx-on*          | Lida com eventos com scripts inline nos elementos                         |
| hx-push-url     | Insere uma URL na barra de localização do navegador para criar histórico  |
| hx-select       | Seleciona o conteúdo a ser substituído a partir de uma resposta           |
| hx-select-oob   | Seleciona o conteúdo a ser substituído a partir de uma resposta, em algum lugar diferente do alvo (fora de banda) |
| hx-swap         | Controla como o conteúdo será substituído (outerHTML, beforeend, afterend, etc.) |
| hx-swap-oob     | Marca o elemento para ser substituído a partir de uma resposta (fora de banda) |
| hx-target       | Especifica o elemento alvo a ser substituído                              |
| hx-trigger      | Especifica o evento que aciona a solicitação                              |
| hx-vals         | Adiciona valores para enviar com a solicitação (formato JSON)             |


### htmx Additional Attributes

| Atributo           | Descrição                                                                 |
|--------------------|---------------------------------------------------------------------------|
| hx-boost           | Adiciona aprimoramento progressivo para links e formulários               |
| hx-confirm         | Exibe um diálogo de confirmação antes de fazer uma solicitação            |
| hx-delete          | Envia uma solicitação DELETE para a URL especificada                      |
| hx-disable         | Desativa o processamento do htmx para o nó e seus nós filhos              |
| hx-disabled-elt    | Adiciona o atributo disabled aos elementos especificados durante uma solicitação |
| hx-disinherit      | Controla e desativa a herança automática de atributos para nós filhos      |
| hx-encoding        | Altera o tipo de codificação da solicitação                               |
| hx-ext             | Extensões a serem usadas para este elemento                               |
| hx-headers         | Adiciona cabeçalhos que serão enviados com a solicitação                  |
| hx-history         | Impede que dados sensíveis sejam salvos no cache de histórico             |
| hx-history-elt     | Elemento a ser capturado e restaurado durante a navegação no histórico    |
| hx-include         | Inclui dados adicionais nas solicitações                                  |
| hx-indicator       | Elemento que recebe a classe htmx-request durante a solicitação           |
| hx-inherit         | Controla e habilita a herança automática de atributos para nós filhos, se desativada por padrão |
| hx-params          | Filtra os parâmetros que serão enviados com uma solicitação               |
| hx-patch           | Envia uma solicitação PATCH para a URL especificada                       |
| hx-preserve        | Especifica elementos a serem mantidos inalterados entre solicitações      |
| hx-prompt          | Exibe um prompt antes de enviar uma solicitação                           |
| hx-put             | Envia uma solicitação PUT para a URL especificada                         |
| hx-replace-url     | Substitui a URL na barra de localização do navegador                      |
| hx-request         | Configura vários aspectos da solicitação                                  |
| hx-sync            | Controla como as solicitações feitas por diferentes elementos são sincronizadas |
| hx-validate        | Força os elementos a se validarem antes de uma solicitação                |
| hx-vars            | Adiciona valores dinamicamente aos parâmetros a serem enviados com a solicitação (obsoleto, use hx-vals) |

### htmx CSS Classes
    - htmx-added
Applied to a new piece of content before it is swapped, removed after it is settled.

    - htmx-indicator
A dynamically generated class that will toggle visible (opacity:1) when a htmx-request class is present

    - htmx-request
Applied to either the element or the element specified with hx-indicator while a request is ongoing

    - htmx-settling
Applied to a target after content is swapped, removed after it is settled. The duration can be modified via hx-swap.

    - htmx-swapping
Applied to a target before any content is swapped, removed after it is swapped. The duration can be modified via hx-swap.

