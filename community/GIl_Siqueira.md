<!-- Título da apresentação -->
# Minha Apresentação - Gilvando Siqueira

<!-- Slide 1 -->
## Quem sou eu?
- Olá!
- Meu nome é Gilvando.
- Sou analista de dados.
- Atuo como analista de gestão em Saúde.

<!-- Slide 2 -->
## Minha jornada
- Comecei a trabalhar com análise de dados há 5 anos.
- Atualmente, estou me especializando em machine learning.

<!-- Slide 3 -->
## Minhas habilidades
- Linguagens de programação:
  - Python
  - SQL
  - PLSQL
  - R

<!-- Slide 4 -->
## Obrigado!
- Obrigado por assistir a minha apresentação!

<style>

section {
  position: absolute;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  opacity: 0;
  transform: translateY(20px);
  transition: opacity 1s, transform 1s;
}

section.active {
  opacity: 1;
  transform: translateY(0);
}
</style>

<script>

const sections = document.querySelectorAll('section');
let index = 0;

function showSlide(index) {
  sections.forEach((section, i) => {
    if (i === index) {
      section.classList.add('active');
    } else {
      section.classList.remove('active');
    }
  });
}

showSlide(index);

document.addEventListener('keydown', (event) => {
  if (event.key === 'ArrowRight' || event.key === 'ArrowDown') {
    index = Math.min(index + 1, sections.length - 1);
    showSlide(index);
  } else if (event.key === 'ArrowLeft' || event.key === 'ArrowUp') {
    index = Math.max(index - 1, 0);
    showSlide(index);
  }
});
</script>
