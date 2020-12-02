<template>
  <div class="px-2">
    <img src="/test.svg" alt="tipos-influencers-marketing-155.svg">
    <div class="text-center mt-2">
        <a class="text-2xl text-blue-400" :href="url" rel="bookmark"> {{titulo}} </a>
    </div>
    <p class="text-center italic">
        16 octubre,2020
    </p>
  </div>
</template>

<script>
export default {
props:['titulo'],

computed:{ 
  url: function(){
    return 'http://google.com/'+this.$router.currentRoute.fullPath;
  }
},

}
</script>

<style>

</style>