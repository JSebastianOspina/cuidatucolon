<template>
  <div class="flex justify-between azul-copia" style="font-family: Helvetica">
    <div class="flex ">
        <div class="">
          <img src="/logo-aulacm.png" class="h-20 w-20" alt="" />
        </div>
        <div class="flex items-center">
          <p class="font-medium text-2xl text-white ">AULA CM</p>
        </div>
    </div>
    <div class="flex items-center mr-5 ">
      <svg
        height="20"
        viewBox="0 -53 384 384"
        width="28"
        xmlns="http://www.w3.org/2000/svg"
        fill="white"
      >
        <path
          d="M368 154.667969H16c-8.832031 0-16-7.167969-16-16s7.167969-16 16-16h352c8.832031 0 16 7.167969 16 16s-7.167969 16-16 16zm0 0M368 32H16C7.167969 32 0 24.832031 0 16S7.167969 0 16 0h352c8.832031 0 16 7.167969 16 16s-7.167969 16-16 16zm0 0M368 277.332031H16c-8.832031 0-16-7.167969-16-16s7.167969-16 16-16h352c8.832031 0 16 7.167969 16 16s-7.167969 16-16 16zm0 0"
        />
      </svg>
    </div>
    
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentColor: "#f4f5fa",
    };
  },
};
</script>
<style>
.azul-copia{
  background-color: #1cbacc;
}
</style>