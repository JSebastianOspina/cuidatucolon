<template>
  <h1>
      {{this.slug}}
  </h1>
</template>

<script>
export default {
 async asyncData({ params }) {
     
      const slug = params.receta // When calling /abc the slug will be "abc"
      return { slug }
    },

    head() {
      return {
        title: this.slug,
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: 'Receta de '+this.slug,
          },
           {
            hid: 'og:description',
            name: 'og:description',
            content: 'Receta de '+this.slug,
          }
        ]
      }
      },
}
</script>

<style>

</style>