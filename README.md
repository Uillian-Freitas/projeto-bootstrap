🍽️ Projeto Restaurante — Bootstrap + jQuery
📌 Objetivo

Criar uma página de restaurante responsiva usando Bootstrap 5 e jQuery, incluindo:

Navegação com scroll

Carousel de imagens

Cardápio com abas dinâmicas

Formulário com validação e máscara de telefone

Estilização personalizada em CSS

🧱 Tecnologias utilizadas
Tecnologia	Função no projeto
HTML5	Estrutura da página
CSS3	Estilo visual
Bootstrap 5.3	Layout responsivo, componentes (navbar, carousel, tabs, formulário)
Bootstrap Icons	Ícones visuais
jQuery 3.7	Manipulação do DOM
jQuery Mask Plugin	Máscara para telefone
jQuery Validation Plugin	Validação do formulário
🗂️ Estrutura do projeto
📁 projeto-restaurante
 ├── index.html
 ├── main.css
 └── 📁 images
      ├── slides
      ├── eventos
      └── cardapio

⚙️ Funcionalidades implementadas
🧭 Navegação

Menu fixo no topo

Scroll suave para seções

Links para:

Sobre o restaurante

Eventos

Cardápio

Contato

🎞️ Carousel

Imagens rotativas automaticamente

Controles “anterior” e “próximo”

📋 Cardápio em abas (Bootstrap Tabs)

Categorias:

Bebidas não alcoólicas

Bebidas alcoólicas

Entradas

Pratos principais

Sobremesas

Cada botão usa:

data-bs-toggle="tab"
data-bs-target="#id-da-aba"

📝 Formulário de Contato

Campos:

Nome (obrigatório)

E-mail (obrigatório e validado)

Telefone (opcional, mas com máscara)

Mensagem (obrigatório)

📞 Máscara de telefone (jQuery)
$('#telefone').mask('(00) 00000-0000');

✅ Validação do formulário (jQuery Validate)
$('form').validate({
    rules: {
        nome: { required: true, minlength: 3 },
        email: { required: true, email: true },
        mensagem: { required: true, minlength: 5 },
        telefone: { digits: true, minlength: 11 }
    },
    messages: {
        nome: "Digite pelo menos 3 letras",
        email: "Digite um e-mail válido",
        mensagem: "A mensagem precisa ter no mínimo 5 caracteres",
        telefone: "Digite um telefone válido com DDD"
    }
});

🎨 Estilização

Fonte padrão: Roboto

Títulos: Pacifico

Cor principal do layout: #e15f41

Botões com efeito de hover e animação de escala

🚀 Resultado final

Página totalmente responsiva

Cardápio funcional com troca de abas

Formulário validado e estilizado

Layout limpo e profissional
