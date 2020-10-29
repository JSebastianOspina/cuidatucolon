<template>
  <div class="h-full flex flex-col inicio">
    <div
      class="bg-cover relative"
      style="height: 65%; background-image: url('/welcome/fondo1.jpg')"
    >
      <div class="custom-shape-divider-bottom-1603982097">
        <svg
          width="437"
          height="553"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          xmlns:svgjs="http://svgjs.com/svgjs"
          viewBox="0 0.598 437 551.805"
          preserveAspectRatio="none"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="437"
            height="553"
            viewBox="90 0.819 436.921 551.705"
          >
            <path
              paint-order="stroke fill markers"
              fill-rule="evenodd"
              d="M90 312.318s58.357-128.75 215.932-84.552C463.507 271.964 513.547.819 513.547.819l13.374 551.705H90V312.318z"
              class="shape-fill"
            />
          </svg>
        </svg>
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
            to="/welcome/1"
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
 

.custom-shape-divider-bottom-1603982097 {
  position: absolute;
  bottom: 0;
  right: 0px;
  overflow: hidden;
  line-height: 0;
  width: 100%;
}

.custom-shape-divider-bottom-1603982097 svg {
  position: relative;
  display: block;
  width: 105%;
  height: 150px;
}

.custom-shape-divider-bottom-1603982097 .shape-fill {
  fill: #f4f5fa;
}
.inicio{
   font-family: 'Open Sans', sans-serif;
}
</style>