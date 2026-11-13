# Meu Portfólio Pessoal

**Aluno:** Tiago Miguel Ferreira Homan

## Sobre o portfólio

Este é o meu portfólio pessoal. Nele eu me apresento, mostro alguns
dos projetos que fiz no curso Técnico em Desenvolvimento de Sistemas
da ETEC e deixo meus contatos. Parti do site que fizemos em aula e
fui melhorando por conta própria.

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Bootstrap 5
- GitHub e GitHub Pages

## Site publicado

https://tiagohoman.github.io/Portfolio/

## Como o site funciona

O site é uma página única, com um menu fixo no topo. Cada item do
menu leva para uma parte da página:

- **Perfil:** uma apresentação sobre mim, o que estudo e o que quero
  para o futuro.
- **Projetos:** quatro cards com trabalhos que fiz. O botão
  "Ver projeto" de cada um abre a pasta do projeto no GitHub.
- **Contato:** meu email, meu WhatsApp e o link do meu GitHub.

O menu usa links de âncora (por exemplo, `href="#projetos"`), que
levam até a seção com o `id` igual. O Bootstrap cuida do layout dos
cards, do menu que vira botão no celular e de deixar o site
responsivo.

## Recursos novos

Além do que vimos em aula, eu adicionei:

1. **Efeito nos cards:** quando o mouse passa por cima, o card sobe
   um pouco e ganha sombra.
2. **Rolagem suave:** ao clicar no menu, a página desliza até a
   seção em vez de pular.
3. **Seções que aparecem aos poucos:** Projetos e Contato surgem com
   um efeito de fade quando chegam na tela.

## Como eu fiz cada recurso

- **Efeito nos cards:** usei `transition` junto com `:hover` no CSS.
  No hover, o card ganha `transform: translateY(-8px)` e
  `box-shadow`. A `transition` faz a mudança acontecer devagar.
- **Rolagem suave:** coloquei `scroll-behavior: smooth` no `html`.
- **Fade nas seções:** as seções começam invisíveis
  (`opacity: 0`) por causa da classe `reveal`. Com JavaScript, usei
  o `IntersectionObserver`, que avisa quando a seção entra na tela.
  Nesse momento ele adiciona a classe `visivel`, e o CSS faz a
  seção aparecer com `transition`.
