# ololjaguars
Quando a largura da tela é menor que 1180px, o menu de navegação desktop é ocultado usando a classe "hide_desktop". Quando a largura da tela é menor que 480px, o menu de navegação inteiro é ocultado usando CSS.

O código JS usa jQuery para criar um menu de navegação dropdown a partir do menu de navegação completo. Ele seleciona o elemento com o ID "section_navigation" e cria um elemento <select> , fora da div"section_navigation", com ID "section_select" e classe "hide_desktop". Em seguida, ele itera sobre cada link dentro do elemento "#section_navigation", cria uma opção <option> para cada link e adiciona a opção ao elemento <select>.

O código adiciona o elemento <select> após o elemento "#section_navigation" usando o método insertAfter() do jQuery. Em seguida, ele adiciona um manipulador de eventos change() ao elemento <select> para atualizar a URL com a seção selecionada e carregar a seção correspondente usando AJAX em uma div com classe "js-mod".
Por fim, o código CSS oculta o menu de navegação desktop em telas menores que 1180px e a navegação inteira em telas menores que 480px, para que o menu de navegação dropdown seja exibido apenas nessas telas menores.

Na linha: $("#sn_content").load(newUrl + " #sn_content > *");. 

Essa linha de código carrega o conteúdo de uma página da web na div com id "sn_content", usando a função jQuery ".load()". A URL da página que será carregada é especificada pela variável "newUrl". O trecho " #sn_content > *" indica que apenas o conteúdo da div com id "sn_content" deve ser carregado na página atual, substituindo o conteúdo existente na div.

Antes estava sendo usado a class. Alterei para ID, porque fica mais consistente e evita bugs na página
