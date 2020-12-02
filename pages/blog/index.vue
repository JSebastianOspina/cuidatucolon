<template>
  <div>
    <div v-for="item in articulos" :key="item.slug">
      <nuxt-link :to="item.slug"> {{item.slug}}</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ $content }) {
    const articulos = await $content("blog").fetch();
    console.log(articulos);
    return { articulos };
  },
};
</script>

<style>
</style>