<template>
<div>
  <div id="navTitle"> 
      <h1 @click="home()"><i class="fas fasi fa-blog"></i> Blog</h1>
  </div>
  <div id="nav"> 
    <h1 @click="home()" class="navTitleInLine" :class="{navTitleInLineHover: aplicar}">Início</h1> 
    <!-- <h1 @click="acupuntura()" class="navTitleInLine" :class="{navTitleInLineHover: aplicarTwo}">Acupuntura</h1> -->
    <h1 @click="lesoes()" class="navTitleInLine" :class="{navTitleInLineHover: aplicarTree}">Lesões</h1>
    <!-- 
    <h1 @click="biomecanica()" class="navTitleInLine" :class="{navTitleInLineHover: aplicarFour}">Biomecânica</h1>
    <h1 @click="treinamento()" class="navTitleInLine" :class="{navTitleInLineHover: aplicarFive}">Treinamento</h1> -->
  </div>
  <div class="main">
    <div v-html="content"></div>
  </div>
  <Footer/>
</div>
</template>
<script>
export default {
  head: {
    title: 'Blog | Professor Leandro Cesar',
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
  },
  data() {
    return {
      content: `
      <h1>Em construção!!</h2>
      <!-- <a href="https://blog.leandrocesar.co/lesoes/joelho-lca">Lesões de Joelho - Ligamento Cruzado Anterior (LCA)</a> -->
      `,
      aplicar: true,
      aplicarTwo: false,
      aplicarTree: false,
      aplicarFour: false,
      aplicarFive: false,
    }
  },
  methods: {
    home() {
      this.content = `
      <h1>Em construção!!</h2>
      <!-- <a href="https://blog.leandrocesar.co/lesoes/joelho-lca">Lesões de Joelho - Ligamento Cruzado Anterior (LCA)</a> -->
      `,
      this.aplicar= true,
      this.aplicarTwo= false,
      this.aplicarTree= false,
      this.aplicarFour= false,
      this.aplicarFive= false
    },
    acupuntura() {
      this.content = `
      
      `,
      this.aplicar= false,
      this.aplicarTwo= true,
      this.aplicarTree= false,
      this.aplicarFour= false,
      this.aplicarFive= false
    },
    lesoes() {
      this.content = `
      <h1>Em construção!!</h2>
      <!-- <a href="https://blog.leandrocesar.co/lesoes/joelho-lca">Lesões de Joelho - Ligamento Cruzado Anterior (LCA)</a> -->
      `,
      this.aplicar= false,
      this.aplicarTwo= false,
      this.aplicarTree= true,
      this.aplicarFour= false,
      this.aplicarFive= false
    },
    biomecanica() {
      this.content = `
      
      `,
      this.aplicar= false,
      this.aplicarTwo= false,
      this.aplicarTree= false,
      this.aplicarFour= true,
      this.aplicarFive= false
    },
    treinamento() {
      this.content = `

      `,
      this.aplicar= false,
      this.aplicarTwo= false,
      this.aplicarTree= false,
      this.aplicarFour= false,
      this.aplicarFive= true
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

#navTitle h1{
    font-weight: bold;
    color: #fadb41;
    display: inline;
    transition: all 0.24s linear;
    cursor: pointer;
    font-size: 2.2em;
}

#navTitle a.nuxt-link-exact-active {
    color: #fadb41;
}

#nav {
    display: flex;
    flex-flow: row wrap;
    align-items: center;
    justify-content:space-around;  
    align-self: center;
    padding: 0 0 15px 0;
    width: 50%;
    margin: auto;
    text-align:center;
}

.navTitleInLine {
    font-weight: bold;
    color: #d8d8d890;
    display: inline;
    transition: all 0.24s linear;
    font-size: 1.3em;
    cursor: pointer;
    padding: 0 5px 0 5px;
}

.navTitleInLineHover {
    color: #fadb41;
    text-decoration: underline;  
}

.navTitleInLine:hover {
    color: #fadb4190;
}
@media only screen and (max-width: 1125px) {
  #nav {
    width: 60%
  }
}
</style>