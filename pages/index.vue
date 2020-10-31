<template >
  <div class="flex flex-col w-screen mt-16">
    <div class="flex justify-around">
      <div class="">
        <span class="text-2xl font-extrabold block">Actividad</span>
      </div>
      <div class="flex items-center">
        <span class="">Hoy, 2 de ocutubre</span>
      </div>
    </div>
    <div class="flex flex-col h-40 py-5 px-6">
      <div class="tarjeta px-1 py-4 bg-white shadow-xl rounded-xl">
        <div class="w-100 ml-4 mb-3">
          <h3 class="text-lg font-bold">Estadísticas</h3>
        </div>
        <div class="flex w-full justify-around">
          <div class="flex-auto pl-3">
            <h3 class="text-sm text-left">Desayunos</h3>
            <p class="text-green-500 text-2xl font-medium">6</p>
          </div>
          <div class="flex-auto pl-3">
            <h3 class="text-sm">Almuerzos</h3>
            <p class="text-green-500 text-2xl font-medium">6</p>
          </div>
          <div class="flex-auto pl-3">
            <h3 class="text-sm">Comidas</h3>
            <p class="text-green-500 text-2xl font-medium">6</p>
          </div>
        </div>
        <div class="text-center text-sm mt-3">
          <p class="inline">Nunca te rindas, la recompensa vendrá</p>
          <span class="text-green-500">pronto</span>
        </div>
      </div>
    </div>
    <div class="flex justify-around mt-10 text-center mx-5">
      <div class="flex-auto py-2 px-5 mx-2 hover:bg-green-400 hover:text-white">
        Desayuno
      </div>
      <div class="flex-auto py-2 px-5 mx-2 hover:bg-green-400 hover:text-white">
        Almuerzos
      </div>
      <div class="flex-auto py-2 px-5 mx-2 hover:bg-green-400 hover:text-white">
        Comidas
      </div>
    </div>

    <div class="flex flex-col bg-red-200 mb-5"  v-for="i in recetas"
        :key="i">
      <div
        :style="{ backgroundImage: s(i.image) }"
        class="h-64 w-2/5 my-3 block bg-cover self-center rounded-xl shadow-xl"
      ></div>
      <div class="text-center">
        <span>{{i.nombre}}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "insideapp",
  methods: {
    s(param) {
      console.log(param);
      return "url(" + param + ")";
    },
  },
  computed: {},
  data() {
    return {
      recetas: [
        {
          nombre: "Hola",
          image:
            "https://cdn5.recetasdeescandalo.com/wp-content/uploads/2019/08/Aprende-como-hacer-un-huevo-frito-perfecto-con-trucos-y-consejos.jpg",
        },
        {
          nombre: "Hola",
          image:
            "https://cdn5.recetasdeescandalo.com/wp-content/uploads/2019/08/Aprende-como-hacer-un-huevo-frito-perfecto-con-trucos-y-consejos.jpg",
        },
        {
          nombre: "Hola",
          image:
            "https://cdn5.recetasdeescandalo.com/wp-content/uploads/2019/08/Aprende-como-hacer-un-huevo-frito-perfecto-con-trucos-y-consejos.jpg",
        },
      ],
    };
  },
};
</script>

<style>
.custom-shape-divider-bottom-1603949143 {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  transform: rotate(180deg);
}

.custom-shape-divider-bottom-1603949143 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 54px;
  transform: rotateY(180deg);
}

.custom-shape-divider-bottom-1603949143 .shape-fill {
  fill: #62b776;
}

/** For mobile devices **/
@media (max-width: 767px) {
  .custom-shape-divider-bottom-1603949143 svg {
    width: calc(100% + 1.3px);
    height: 54px;
  }
}
</style>