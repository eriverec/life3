<template>
  <div v-editable="blok" class="margin-b">
    <div>
      <div class="uk-card uk-card-primary uk-card-body center__margin">
      <img :src="resizeImage" class="is"/>
        <h3 class="uk-card-title">{{ blok.titulo }}</h3>
        <p>{{ blok.intro }}</p>

        <h4> {{blok.direccion}} </h4>
      </div>
    </div>
  </div>
</template>

<script>
import Filter from '~/plugins/filters'
export default {
  props: ["blok"],
  computed: {
    resizeImage(){
      const imageUrl = this.blok.hero_image
      if (typeof imageUrl !== 'undefined'){
        return imageUrl.filename.replace('//a.storyblok.com','//img2.storyblok.com/300x250')
      }
      return null
    }
  }
};
</script>

