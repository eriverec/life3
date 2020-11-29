<template>
  <div v-editable="blok">
    <div>
      <h2> {{blok.titulo}} </h2>
    </div>
    <ul>
      <li 
      v-for="articulo in blok.articulos"
      :key="articulo._uid">

      <articulo
        v-if="articulo.content"
        :articulo-content="articulo.content"/>

      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
};
</script>
