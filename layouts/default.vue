<template>
  <div class="h-full flex flex-col">
    <div>
      <img class="md:h-40 w-full" src="/wave.svg" alt="" />
      <img
        class="md:h-40 w-full absolute"
        style="top: 5px"
        src="/wave copy.svg"
        alt=""
      />
    </div>

    <Nuxt />

    <div>
      <img
        class="h-16 sm:h-20 w-full absolute"
        style="bottom: 0px"
        src="/wave-inverted.svg"
        alt=""
      />
      <img
        class="h-16 sm:h-20 w-full absolute"
        style="bottom: 7px"
        src="/wave-inverted copy.svg"
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
