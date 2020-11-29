<template>
  <div>
  <nav>
      <ul class="menuItems animate__animated animate__fadeInDown">
        <li v-for="(item, i) in items" :key="i">
          <NuxtLink router exact :to="item.to">
            {{ item.title }}
          </NuxtLink>
        </li>
      </ul>
    </nav>
    <Nuxt />
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "Life",
      items: [
        {
          title: "Home",
          to: "/"
        },
        {
          title: "Campos",
          to: "/camp"
        },
        {
          title: "Educación",
          to: "/educ"
        },
        {
          title: "Experiencia",
          to: "/exp"
        },
        {
          title: "Referencias",
          to: "/refer"
        },
        {
          title: "Conocimientos",
          to: "/conoc"
        }
      ]
    };
  },

};
</script>

<style>
html {
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

body {
  font-family: "Montserrat", sans-serif !important;
}

.teaser,
.column {
  font-size: 2rem;
  text-align: center;
  line-height: 3;
  background: #ebeff2;
  border-radius: 10px;
  margin: 10px 5px;
}

.grid {
  display: flex;
}

.column {
  flex: 1;
}
</style>