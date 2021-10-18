<template>
<div>
  <Nav/>
  <div id="main" class="nav-in">
        <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
      </div>
    <div id="main">
      <p>
          Em Construção!
      </p>
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
  }
} 
</script>


<style>

</style>