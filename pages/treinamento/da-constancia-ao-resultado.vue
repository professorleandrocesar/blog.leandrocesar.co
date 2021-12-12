<template>
<div>
  <div id="navTitle"> 
      <NuxtLink to="/"><i class="fas fasi fa-blog"></i> Blog</NuxtLink>
  </div>
  <div>
    <div id="main" class="nav-in"> 
      <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
      <br>
    </div>
    <div id="main">
    
      <!-- Início Cabeçalho principal da página -->
      <h1>{{postTitle}} </h1><h3> {{subPostTitle}}</h3>
      <h5 class="main-r">Autor: {{autor}}
        <br>Criado:
        <i class="far fa-calendar-minus"></i> {{date}}  <i class="far fa-clock"></i> {{hours}}
        <!--<br>Editado:
        <i class="far fa-calendar-minus"></i> {{oneReeditionDate}}  <i class="far fa-clock"></i> {{oneReeditionHours}} -->
      </h5>
      <!-- Fim Cabeçalho principal da página -->


      <!-- Início do conteúdo principal -->
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
      <!-- Fim do Conteúdo principal da página -->
    
    
    </div>
  </div>
  <div id="main" class="nav-in"> 
    <br>
      <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
    <br>
  </div>
  <Footer/>
</div>
</template>
<script>
export default {
data() {
  return {
    postTitle: 'Da Constância ao Resultado:',
    subPostTitle: ' O Princípio da Continuidade no Treinamento Físico', /* deixar com um espaço inicial */
    area: ' | Blog', /* deixar com um espaço inicial - Colocar a area da postagem */
    autor: ' Professor Leandro Cesar', /* deixar com um espaço inicial */
    descript: '', /* descrição de no máximo 200 caracteres */
    key: ', , ', /* colocar 3 keywords */
    date: '',
    hours: '',
    oneReeditionDate: '',
    oneReeditionHours: ''
  }
},
head() {
  return {
      title: [this.postTitle + this.subPostTitle + ' |' + this.area + ' |' + this.autor],
        meta: [
        {
          hid: 'description',
          name: 'description',
          content: [this.descript]
        },
        {
          hid: 'keywords',
          name: 'keywords',
          content: [this.key]
        }
      ]       
    }
  }
}
</script>

<style>
#navTitle {
  padding: 30px 0 10px 0;
  font-size: 1em;
  text-align: center;
  /* 
  Para colocar barra fixa:
  position: fixed;
  top: 0;
  margin: auto;
  height: 50px;
  width: 100%; */
}

#navTitle a{
  font-weight: bold;
  color: #fadb41;
  display: inline;
  transition: all 0.24s linear;
  cursor: pointer;
  font-size: 2.2em;
}
</style>