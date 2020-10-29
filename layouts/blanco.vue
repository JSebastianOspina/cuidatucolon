<template >
  <div class="contenedor h-screen">
       <Nuxt />
  </div>
</template>
<script>
export default {
  mounted() {
    let vh = window.innerHeight * 0.01;
    // Then we set the value in the --vh custom property to the root of the document
    document.documentElement.style.setProperty("--vh", `${vh}px`);
  },
};
</script>
<style >

body {
  background-color: #f4f5fa;
  position: relative;
}
.contenedor{
height: 100vh; /* Fallback for browsers that do not support Custom Properties */
height: calc(var(--vh, 1vh) * 100);
overflow: hidden;
}
</style>