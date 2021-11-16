<template>
<div>

  <div id="navTitle"> 
      <NuxtLink to="/"><i class="fas fasi fa-blog"></i> Blog</NuxtLink>
  </div>

  <div id="main" class="nav-in"> 
    <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
    <br>
  </div>
  <div id="main">
  
    <!-- Início Cabeçalho principal da página -->
    <h1>{{postTitle}}</h1><h3>{{subPostTitle}}</h3>
    <h5 class="main-r">
      Autor: {{autor}}
      <br>Criado:
      <i class="far fa-calendar-minus"></i> {{date}}  <i class="far fa-clock"></i> {{hours}}
      <!--<br>Editado:
      <i class="far fa-calendar-minus"></i> {{oneReeditionDate}}  <i class="far fa-clock"></i> {{oneReeditionHours}} -->
    </h5>
    <!-- Fim Cabeçalho principal da página -->





      <!-- Início do conteúdo principal -->   
    <p>
      Venho percebendo relatos, de alunos e até de alguns clientes de Personal,
      queixando-se de dores nos joelhos. Na grande maioria das reclamações
      as dores estão localizadas na parte medial (interna) do joelho.
    </p>
    <p>
      Nesta região medial, há uma grande incidência de entorses do Ligamento Cruzado Anterior (LCA);
    <p>
      <blockquote>
      É uma das lesões mais
      comuns na articulação do joelho, com frequência de ocorrência de 5 a 10 vezes maior em 
      relação a lesão de outros ligamentos localizados no joelho<sup> 1</sup>. 
      </blockquote>
      Este texto é um esforço, para melhor entender o complexo articular do joelho, fazendo uma revisão 
      anatômica e mais específicamente entender o ligamento cruzado anterior e sua lesão ligamentar. 
    </p>
    </p>
    <div class='title-link'>
      <h4>
        <NuxtLink to='#revisao-anatomica'>Anatomia</NuxtLink>
      </h4>
    </div>
    <p>
      O joelho é uma articulação sinovial com estruturas bem complexas. É formada pelos ossos do 
      fêmur, tíbia, e patela. Conectados pelos muitos componentes articulares para garantir sua 
      movimentação e estabilidade, permitindo sustentar grandes cargas para a mobilidade, necessárias
      para as atividades locomotoras do dia-a-dia.<sup> 2</sup>.
    </p>
    <div class="legend">
      <img src="/img/articulacao-do-joelho.png" alt="Foto de uma articulação do joelho">
      <br>
      <sub>Corte sagital do Joelho direito (Rasch e Burke, 1986 p.340) <sup> 3</sup></sub>    
    </div>
    <p>

    </p>

    <div class="refer">
      <h6>Referências Bibliográficas:</h6>
      <p>
        1) (Macnicol, 2002)
        <br>
        2) Biomecânica Básica
        <br>
        3) Rasch e bu    
      </p>
    </div>
    <!-- Fim do Conteúdo principal da página -->
    
    


 
    <div id="main" class="nav-in"> 
      <br>
        <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
      <br>
    </div>
  </div>
  <Footer/>
</div>
</template>
<script>
export default {
data() {
  return {
    postTitle: 'Lesões de Joelho:',
    subPostTitle: ' Ligamento Cruzado Anterior (LCA)', /* deixar com um espaço inicial */
    area: ' Lesões | Blog', /* deixar com um espaço inicial */
    autor: ' Professor Leandro Cesar', /* deixar com um espaço inicial */
    descript: '', /* descrição de no máximo 200 caracteres */
    key: ', , ', /* colocar 3 keywords */
    date: '22/11/2021',
    hours: '06:00',
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
  color: #fabf42;
  display: inline;
  transition: all 0.24s linear;
  cursor: pointer;
  font-size: 2.2em;
}

.title-link a{
  color: #fff;
  text-align:left;
}

.title-link a:hover{
  text-decoration: underline;
}

.legend {
    margin: auto;
    text-align: center;
}

.legend img {
    width: 300px;
    height: auto;
    margin-bottom: -15px;
    border: solid 1px #fff; 
    border-radius: 0.3em 0.3em 0.3em 0.3em;
}

.legend sub {
    font-size: .7em;

}

.refer h6 {
        margin-bottom: 15px;
    }

    .refer p {
      font-size: .8em;
    }

</style>