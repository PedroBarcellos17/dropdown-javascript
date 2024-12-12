## Dropdown Simples com HTML, CSS e JavaScript

### Descrição
Este projeto implementa um menu dropdown simples utilizando HTML, CSS e JavaScript. O menu possui uma estrutura básica de navegação com um item principal chamado "Linguagens", que, ao ser interagido, exibe um submenu com links para diferentes linguagens de programação.

Este exemplo visa demonstrar como combinar essas três tecnologias para criar um menu interativo e responsivo.

## Funcionamento

### HTML
O HTML é responsável pela estrutura do menu. Ele utiliza uma lista não ordenada (<ul>) para agrupar os itens do menu. Dentro dessa lista, temos itens de menu (<li>), e um desses itens contém um submenu, que também é uma lista (<ul class="dropdown">), mas é exibido somente quando o usuário passa o mouse sobre o item "Linguagens".

### Estrutura do menu:
O menu é composto por quatro itens principais: "Home", "Linguagens", "Mais sobre a Empresa" e "Contato".
O item "Linguagens" contém um submenu com links para várias linguagens de programação, como HTML, CSS, JavaScript, Python e MySQL.
Submenu:
O submenu fica oculto por padrão e só é exibido quando o item "Linguagens" é "hovered" (passado o mouse sobre ele). Isso é controlado pelo CSS.
###CSS
O CSS é responsável pela aparência visual e pelo comportamento do menu. Ele define o layout, as cores e as transições, além de controlar a exibição do submenu quando o usuário interage com o item "Linguagens".

## Estilo básico do menu:

O menu tem uma cor de fundo azul escuro (#22438C) e os itens de menu são apresentados horizontalmente.
Cada item de menu tem um espaço definido (padding) e uma cor de texto branca, proporcionando uma boa legibilidade.
Hover:

Quando o usuário passa o mouse sobre um item de menu, a cor de fundo do item muda, dando um feedback visual de interação.
Submenu oculto:

O submenu (dentro do <ul class="dropdown">) está inicialmente escondido com a regra display: none.
Quando o item "Linguagens" é "hovered", a regra display: block é aplicada ao submenu, tornando-o visível.
Posicionamento do submenu:

O submenu é posicionado absolutamente em relação ao item de menu "Linguagens", aparecendo abaixo dele quando visível.
### JavaScript
O JavaScript (caso tenha sido incluído) pode ser usado para adicionar interatividade mais avançada ao menu, como animações, transições, ou até mesmo controle de visibilidade do submenu em dispositivos móveis. Embora o código apresentado não utilize JavaScript diretamente, ele poderia ser utilizado para:

Adição de animações: Como transições suaves para exibir ou ocultar o submenu.
Controle de visibilidade em dispositivos móveis: Em vez de usar apenas o hover, o JavaScript poderia ser utilizado para alternar a visibilidade do submenu com um clique, o que é mais adequado para dispositivos móveis onde o hover não funciona.
## Resumo do Funcionamento
HTML: Estrutura a navegação, criando os itens de menu e o submenu.
CSS: Estiliza o menu e controla a visibilidade do submenu com base na interação do usuário (hover).
JavaScript (opcional): Pode ser adicionado para fornecer animações ou controle avançado sobre o comportamento do menu, como alternar a visibilidade ao clicar, especialmente em dispositivos móveis.
Como Funciona a Interação do Usuário
Quando o usuário passa o mouse sobre o item Linguagens, o submenu aparece com uma lista de linguagens.
A cor de fundo do item de menu muda para um tom mais escuro quando o usuário passa o mouse sobre ele, dando um feedback visual de interação.
Ao mover o mouse para fora do item "Linguagens", o submenu desaparece.
Personalização
Você pode ajustar a aparência e o comportamento do menu de acordo com suas necessidades:

Estilos: Modifique as cores, fontes e tamanhos no CSS para se alinhar com a identidade visual do seu projeto.
Interatividade: Adicione JavaScript para introduzir animações, controles de clique ou outras interações personalizadas.

Este exemplo simples de dropdown pode ser expandido para incluir mais funcionalidades, como menus multi-nível ou controles adaptativos para dispositivos móveis.
