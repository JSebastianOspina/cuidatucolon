<template>
  <div class="h-full flex flex-col inicio">
    <div
      class="bg-cover relative"
      style="height: 65%; background-image: url('/welcome/fondo1.jpg')"
    >
      <div class="custom-shape-divider-bottom-1">
      <svg viewBox="0 0 500 150" preserveAspectRatio="none" ><path class="shape-fill" d="M-100.24,170.19 C90.82,20.98 450.96,301.27 500.22,0.30 L513.77,153.25 L0.79,172.00 Z"></path></svg>
      </div>
    </div>

    <div class="flex-1 flex items-center">
      <div class="text-center px-6">
        <h2 class="font-black text-2xl mb-3 tracking-wide">1) Desintoxicación</h2>
        <p class="font-light text-sm text-gray-600 ">
          La clave para mejorar tu situacion es mejorar tu alimentación.
          Descubre recetas ricas y saludables que te ayudarán en el proceso.
        </p>
        <div class="mt-6 flex justify-between">
           <nuxt-link to="/welcome" class="text-gray-500  px-8 py-3"
            >Atrás</nuxt-link
          >

          <nuxt-link
            to="/"
            class="bg-green-500 text-white px-8 py-3 rounded-xl"
            >Siguiente</nuxt-link
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "blanco",
  transition: {
    name: 'steps',
  }
};
</script>
<style >
 

.custom-shape-divider-bottom-1 {
  position: absolute;
  bottom: 0;
  right: 0px;
  overflow: hidden;
  line-height: 0;
  width: 100%;
}

.custom-shape-divider-bottom-1 svg {
  position: relative;
  display: block;
  width: 100%;
  height: 200px;
}

.custom-shape-divider-bottom-1 .shape-fill {
  fill: #f4f5fa;
}
.inicio{
   font-family: 'Open Sans', sans-serif;
}
</style>