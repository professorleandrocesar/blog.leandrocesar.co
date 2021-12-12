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
      <p>

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
    postTitle: '',
    subPostTitle: ' ', /* deixar com um espaço inicial */
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