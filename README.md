## Sistema de Abas (Tabs) com HTML, CSS e JavaScript

###Descrição
Este projeto implementa um sistema de abas interativas (tabs) usando HTML, CSS e JavaScript. O layout apresenta um conjunto de abas na parte superior, e cada aba, quando clicada, exibe um conteúdo relacionado, com uma imagem e uma descrição.

Este exemplo mostra como integrar essas três tecnologias para criar uma navegação simples e interativa entre diferentes seções de conteúdo.

## Funcionamento

### HTML
O HTML é responsável pela estrutura do sistema de abas. Ele contém:

Estrutura de Botões: Uma lista de botões, onde cada botão representa uma aba. Cada botão possui um atributo content-id, que é usado para identificar qual conteúdo será exibido quando a aba for clicada.
Conteúdos das Abas: Para cada aba, há uma seção de conteúdo associada. As seções de conteúdo têm a classe content e possuem identificadores exclusivos que correspondem aos valores de content-id dos botões. Essas seções contêm uma imagem e um texto explicativo.
Cada aba está representada por um botão <button> dentro da div com a classe .tab-buttons, e o conteúdo de cada aba está dentro da div .tab-content.

### CSS
O CSS é responsável pela aparência visual e pelo comportamento interativo das abas e do conteúdo exibido. Ele estiliza a interface e controla como as abas são apresentadas e como o conteúdo é exibido ou ocultado:

Estrutura das Abas:

Os botões das abas são estilizados para ficarem alinhados horizontalmente usando a propriedade display: flex na classe .tab-buttons.
Cada botão tem um fundo claro e, ao ser clicado (ou "hovered"), a cor de fundo muda para fornecer feedback visual ao usuário.
O botão ativo, representando a aba atualmente selecionada, recebe uma cor de fundo diferente (background-color: #c7d2fe), e essa cor muda suavemente com uma transição (transition: background-color .3s ease).
Conteúdo das Abas:

O conteúdo de cada aba é inicialmente oculto, utilizando a classe .content, que possui a propriedade display: none.
Quando uma aba é clicada, a classe .show é aplicada à seção correspondente, tornando-a visível com display: flex. A classe .show também aplica estilos adicionais para espaçamento, cor de fundo e bordas arredondadas.
Design Responsivo:

O design é centrado na tela usando display: flex no body, garantindo que o conteúdo do sistema de abas se ajuste de forma flexível no centro da página.
As imagens são ajustadas para ocupar 50% da largura da área de conteúdo e possuem uma altura fixa.

### JavaScript
O JavaScript é responsável pela interatividade das abas. Ele lida com a troca de abas e com a exibição do conteúdo correto quando um botão de aba é clicado.

Seleção de Abas:
O código seleciona todos os botões de aba usando document.querySelectorAll('.tab-btn'). Em seguida, ele adiciona um ouvinte de eventos a cada botão para detectar cliques.
Função tabClicked:
Quando um botão é clicado, a função tabClicked é acionada. Ela faz duas coisas principais:
Remove a classe active de todos os botões e a adiciona ao botão clicado, para indicar que ele está ativo.
Remove a classe show de todas as seções de conteúdo e a adiciona à seção de conteúdo correspondente ao botão clicado, tornando o conteúdo visível.

## Inicialização:

Ao carregar a página, a primeira aba já é exibida. Isso é feito selecionando o botão com a classe active e chamando a função tabClicked para exibir o conteúdo correspondente à aba ativa.
Como Funciona a Interação do Usuário
Quando o usuário clica em uma das abas (como "Home", "Services", "Contacts", etc.), o JavaScript altera a aba ativa e exibe o conteúdo correspondente.
A aba ativa recebe uma cor de fundo diferente, indicando qual seção está visível.
O conteúdo associado à aba clicada é mostrado, enquanto os conteúdos das outras abas permanecem ocultos.
## Personalização

Aparência: Você pode modificar as cores, fontes e o layout do sistema de abas no arquivo CSS. A fonte usada neste exemplo é a fonte "Poppins" do Google Fonts, mas pode ser substituída por qualquer outra fonte ou estilo.
Conteúdo: O conteúdo exibido em cada aba pode ser facilmente alterado, basta modificar as seções de conteúdo no HTML.
Interatividade: Se desejar adicionar novas interações ou animações, o JavaScript pode ser expandido para incluir funcionalidades adicionais, como transições suaves entre os conteúdos ou controle de navegação por teclas.
