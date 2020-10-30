<template >
  <div class="flex flex-col w-screen bg-blue-200">
    <div class="flex superior justify-around">
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
    <div class="flex flex-auto items-center flex-col bg-red-200 ">
      <div v-for="i in 4" :key="i" style="" class="h-64 flex-auto w-2/5 px-20 my-3 rounded-xl shadow-xl bg-yellow-200">
       
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "insideapp",
};
</script>

<style>
.todo {
}
</style>