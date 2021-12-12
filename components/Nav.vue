<template>
<div>
    <div id="navTitle"> 
        <h1><NuxtLink to="/"><i class="fas fasi fa-blog"></i> Blog</NuxtLink></h1>
      </div>
      <div id="nav"> 
        <NuxtLink to="/">Início</NuxtLink> |
        <NuxtLink to="/acupuntura">Acupuntura</NuxtLink>
        <br>
        <NuxtLink to="/lesoes">Lesões</NuxtLink> |
        <NuxtLink to="/biomecanica">Biomecânica</NuxtLink>
      </div>
</div>
</template>

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

#navTitle a {
    font-weight: bold;
    color: #fadb41;
    display: inline;
    transition: all 0.24s linear;
}

#navTitle a.nuxt-link-exact-active {
    color: #fadb41;
}

#nav {
    padding: 10px 0 30px 0;
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

#nav a {
    font-weight: bold;
    color: #d8d8d890;
    display: inline;
    transition: all 0.24s linear;
}

#nav a:hover {
    text-decoration: underline;
}

#nav a.nuxt-link-exact-active {
    color: #fadb41;
    text-decoration: underline;  
}
</style>