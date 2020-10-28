<template>
  <div class="h-screen flex flex-col overflow-hidden">
    <div>
      <img class="md:h-40 w-full" src="wave.svg" alt="" />
      <img
        class="md:h-40 w-full absolute"
        style="top: 5px"
        src="wave copy.svg"
        alt=""
      />
    </div>

    <Nuxt />

    <div class="" style="">
      <img
        class="sm:h-20 w-full absolute"
        style="bottom: 0px"
        src="wave-inverted.svg"
        alt=""
      />
      <img
        class="sm:h-20 w-full absolute"
        style="bottom: 10px"
        src="wave-inverted copy.svg"
        alt=""
      />
    </div>
  </div>
</template>

<style>
body {
  background-color: #f4f5fa;
}
</style>
