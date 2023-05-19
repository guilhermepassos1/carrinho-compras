<script setup>
import {livros} from '@/_data/livros.js'
</script>

<template>
 <h1>minha livraria</h1> 
 <div class="listagem-livros">
 <div class="card-livro" v-for="livro in livros" :key="livro.id">
  <img :src="livro.img" alt="capa do livro" class="capa-livro" />
  <p class="titulo-livro">{{ livro.title }} </p>
  <p class="autor-livro">{{ livro.autor }} </p>
 <p class="preco-livro">{{ livro.preco }} </p>

{{ livros }}
</div>
</div>
<!-- {{ livros }} -->

</template>

<style scoped>
img{
  width: 250px;
}

</style>
