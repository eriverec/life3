<template>
  <div>
    <a href="#">
      <h2>{{articuloContent.titulo}}</h2>
      <p> {{articuloContent.intro}} </p>

    </a>
  </div>
</template>

<script>
export default {
  props:{
    articuloContent:{
      type: Object,
      required: true
    } 
  }
}
</script>


