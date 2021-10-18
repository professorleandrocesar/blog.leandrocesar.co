<template>
    <div>
        <Nav/>
        <div>
            <div id="main" class="nav-in"> 
                <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
            </div>
            <div id="main">
            <h1>Da Constância ao Resultado</h1>
            <h3>O Princípio da Continuidade no Treinamento Físico</h3>
            <h5 class="main-r">Autor: Professor Leandro Cesar
              <br>
              <i class="far fa-calendar-minus"></i> 11/09/2021  <i class="far fa-clock"></i> 09:00
            </h5>
            <p>
               Sabe-se de forma racional e empírica que tudo na vida é conquistado
               com o esforço diário.
               <br>
               E no Treinamento Físico não é diferente!
               <br>
               Através da rotina, da 
               constância é que conseguimos alcançar nossos
               objetivos e assim chegamos num resultado ao 
               qual estava traçado no início do percurso.
            </p>
               <h4>Princípio da continuidade</h4>
            <p>   
              O princípio da continuidade é um dos vários princípios que cercam o treinamendo Físico, a saber
              existe ainda: 
            </p>
            <p>
              <ul>
                <li>Princípio da Individualidade</li>
                <li>Princípia da Variabilidade</li>
                <li>Princípio do Volume/intensidade</li>
                <li>Princípio da Adaptação biológica</li>
                <li>Princípio da Progressão</li>
                <li>Princípio da Sobrecarga</li>
              </ul>            
            </p>
            <p>
              Neste Post, falaremos sobre o Princípio da Continuidade, pela relevância que venho encontrando no dia-a-dia, por cliente de Personal
              Trainer e pelos alunos de musculação;
            </p>
            <h4>Conceitos</h4>
            <p>
              O princípo da continuidade é .... (TUBINO)
            </p>
            <h4>Experiência e contexto</h4>
            <p>
              Para quem não sabe atuo como Profissional de Educação Física, há 13 anos (desde 2008, quando me formei), fora os dois anos que já estagiava
              no setor da musculação, totalizando 15 anos (vide <a href="http://lattes.cnpq.br/3830820363501969">curriculum;</a>).
              <br>
              Sempre observei que 

            </p>
            <p>
              Referências Bibliográficas:
              <br>
              <a href="https://medium.com/@cortexconteudo/a-hist%C3%B3ria-de-m%C3%ADlon-de-crotona-83f26766e334">A história de Mílon de Crotona</a>
            </p>
            </div>
        </div>
        <Footer/>
    </div>  
</template>

<script>
export default {
  head: {
    title: 'Da Constância ao Resultado | Professor Leandro Cesar',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Blog com conteúdos sobre Musculação | Personal Trainer | Consultoria | Acupuntura | Yoga | Professor Leandro Cesar'
      },
      {
        hid: 'keywords',
        name: 'keywords',
        content: 'Personal, Musculação, Acupuntura, Yoga, Professor Leandro Cesar'
      }
    ]
  }
} 
</script>

<style scoped>
a {
  display: inline;
  margin: 0;
}
</style>