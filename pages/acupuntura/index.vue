<template>
<div>
  <Nav/>
  <div>
    <div id="main" class="nav-in">
        <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
      </div>
    <div id="main">
      <p>
          Em Construção!
      </p>
    </div>
  </div>
  <Footer/>
</div>
</template>
<script>
export default {
  head: {
    title: 'Blog | Acupuntura | Professor Leandro Cesar',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Blog | Acupuntura | Professor Leandro Cesar'
      },
      {
        hid: 'keywords',
        name: 'keywords',
        content: 'Acupuntura, Professor Leandro Cesar'
      }
    ]
  }
} 
</script>


<style>

</style>