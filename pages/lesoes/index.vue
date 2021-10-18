<template>
<div>
  <Nav/>
    <div id="main" class="nav-in">
        <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
      </div>
    <div class="main">
    <NuxtLink to="/lesoes/joelho-lca">Lesões de Joelho - Ligamento Cruzado Anterior (LCA)</NuxtLink>
    </div>
  <Footer/>
</div>
</template>
<script>
export default {
  head: {
    title: 'Blog | Lesões | Professor Leandro Cesar',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Blog | Lesões | Professor Leandro Cesar'
      },
      {
        hid: 'keywords',
        name: 'keywords',
        content: 'Lesões, Joelhos, Professor Leandro Cesar'
      }
    ]
  }
} 
</script>


<style>

</style>