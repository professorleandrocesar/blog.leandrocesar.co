<template>
<div>
  <Nav/>
 <div>
    <div id="main" class="nav-in">
        <a @click="$router.go(-1)"><i class="fas main-l fa-arrow-left"></i> Voltar</a>
    </div>
    <br>
    <div id="main">
      <h1>Lesões de Joelho: <br> Ligamento Cruzado Anterior (LCA)</h1>
      <p>Na atualidade, Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit, voluptatem cum obcaecati, rerum facere voluptatibus architecto soluta eveniet iusto, perferendis ab blanditiis officiis unde sit sunt. Optio neque expedita laboriosam. </p>
      <h4>Revisão anatômica</h4>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam minus quia aspernatur at est eligendi debitis autem quibusdam sint maxime, voluptas eius officia quae illum dignissimos, similique, cum labore corrupti.</p>
    </div>
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