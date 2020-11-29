<template>
  <div v-editable="blok">
    <div class="center ">
      <div>{{ blok.headline }}</div>
      <p class="animate__animated animate__fadeInUp">{{ blok.intro }}</p>
      <div>{{ blok.texto }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["blok"]
};
</script>

<style scoped>
p {
  margin: 16px;
  font-size: 96px;
  color: #ccc;
  text-transform: uppercase;
  font-weight: 600;
  transition: all 1s ease-in-out;
  position: relative;
}

.center {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
  text-transform: uppercase;
  text-align: center;
}


@media (max-width: 600px) {
  p {
    font-size: 4em;
  }
}
</style>
