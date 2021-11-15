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
      <h1>{{postTitle}}</h1><h3>{{subPostTitle}}</h3>
      <h5 class="main-r">Autor: {{autor}}
        <br>Criado:
        <i class="far fa-calendar-minus"></i> {{date}}  <i class="far fa-clock"></i> {{hours}}
        <!--<br>Editado:
        <i class="far fa-calendar-minus"></i> {{oneReeditionDate}}  <i class="far fa-clock"></i> {{oneReeditionHours}} -->
      </h5>
      <!-- Fim Cabeçalho principal da página -->


      <!-- Início do conteúdo principal -->
      <p>Na atualidade, Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit, voluptatem cum obcaecati, rerum
    facere voluptatibus architecto soluta eveniet iusto, perferendis ab blanditiis officiis unde sit sunt. Optio neque
    expedita laboriosam. </p>
<h4>Revisão anatômica</h4>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam minus quia aspernatur at est eligendi debitis autem
    quibusdam sint maxime, voluptas eius officia quae illum dignissimos, similique, cum labore corrupti.</p>
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
    postTitle: 'Lesões de Joelho:',
    subPostTitle: ' Ligamento Cruzado Anterior (LCA)', /* deixar com um espaço inicial */
    area: ' Lesões | Blog', /* deixar com um espaço inicial */
    autor: ' Professor Leandro Cesar', /* deixar com um espaço inicial */
    descript: '', /* descrição de no máximo 200 caracteres */
    key: ', , ', /* colocar 3 keywords */
    date: '17/11/2021',
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
</style>