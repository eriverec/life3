<template>
  <div v-editable="blok" class="margin-b">
    <div>
      <div class="uk-card uk-card-primary uk-card-body center__margin">
        <h3 class="uk-card-title">{{ blok.titulo }}</h3>
        <p>{{ blok.intro }}</p>

        <h4> {{blok.direccion}} </h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["blok"]
};
</script>

