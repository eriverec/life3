<template>
  <div v-editable="blok" class=" feature">
    <article class="card">
      <header class="card__thumb">
        <a href="javascript:void(0)"
          ><img
            src="https://images.unsplash.com/photo-1512466699224-9d8217244131?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=4b6f389eb54cb8e27ee8ee5d4040a5d7&dpr=1&auto=format&fit=crop&w=1000&q=80&cs=tinysrgb"
        /></a>
      </header>
      <div class="card__body">
        <div class="card__category"><a href="#">Category</a></div>
        <div class="card__title">
          <h3 href="#">{{ blok.titulo }}</h3>
        </div>
        <p class="card__description">
          {{ blok.texto }}
        </p>
      </div>
    </article>
  </div>
</template>

<script>
export default {
  props: ["blok"]
};
</script>
