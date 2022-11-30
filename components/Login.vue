<template>
  <div class="md:px-32 lg:px-64">
    <h3 class="text-center mt-2 text-4xl font-medium">Bienvenido</h3>

    <div class="text-center px-10">
      <form action="">
        <div class="mt-4">
          <input
            class="py-3 px-5 w-full leading-tight shadow-md text-gray-700"
            type="email"
            name="email"
            id="email"
            placeholder="Correo electrónico"
          />
        </div>
        <div class="mt-10">
          <input
            class="py-3 px-5 w-full leading-tight shadow-md text-gray-700"
            type="password"
            name="contra"
            id="contra"
            placeholder="Contraseña"
          />
        </div>
        <p class="text-md font-light mt-6 text-gray-600 ">¿Olvidaste tu contraseña?</p>
        <nuxt-link to="/welcome">
          <button
            class="mt-6 py-3 rounded-full text-white bg-blue-900 px-7 w-full"
            type="submit"
            @click=""
          >
            Iniciar sesión
          </button>
        </nuxt-link>

        <p class="text-md font-light text-gray-600 mt-6 inline-block">
          ¿No tienes una cuenta?
        </p>
        <a class="ml-1 text-gray-700" href="">Regístrate</a>
      </form>
    </div>
    <div class="flex flex-row mt-5 justify-center">

      <div class="mr-2 p-3 rounded-md shadow-md w-auto bg-white">
        <svg
          class="w-10 rounded h-5 mx-auto"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 512 512"
        >
          <path
            d="M384 176h-96v-64c0-17.664 14.336-32 32-32h32V0h-64c-53.024 0-96 42.976-96 96v80h-64v80h64v256h96V256h64l32-80z"
            fill="#1976d2"
          />
        </svg>
      </div>
      <div class="ml-2 p-3 shadow-md rounded-md w-auto bg-white">
        <svg  class="w-10  h-5 mx-auto" href="http://google.com"
        xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
          <path
            d="M492.668 211.489l-208.84-.01c-9.222 0-16.697 7.474-16.697 16.696v66.715c0 9.22 7.475 16.696 16.696 16.696h117.606c-12.878 33.421-36.914 61.41-67.58 79.194L384 477.589c80.442-46.523 128-128.152 128-219.53 0-13.011-.959-22.312-2.877-32.785-1.458-7.957-8.366-13.785-16.455-13.785z"
            fill="#167ee6"
          />
          <path
            d="M256 411.826c-57.554 0-107.798-31.446-134.783-77.979l-86.806 50.034C78.586 460.443 161.34 512 256 512c46.437 0 90.254-12.503 128-34.292v-.119l-50.147-86.81c-22.938 13.304-49.482 21.047-77.853 21.047z"
            fill="#12b347"
          />
          <path
            d="M384 477.708v-.119l-50.147-86.81c-22.938 13.303-49.48 21.047-77.853 21.047V512c46.437 0 90.256-12.503 128-34.292z"
            fill="#0f993e"
          />
          <path
            d="M100.174 256c0-28.369 7.742-54.91 21.043-77.847l-86.806-50.034C12.502 165.746 0 209.444 0 256s12.502 90.254 34.411 127.881l86.806-50.034c-13.301-22.937-21.043-49.478-21.043-77.847z"
            fill="#ffd500"
          />
          <path
            d="M256 100.174c37.531 0 72.005 13.336 98.932 35.519 6.643 5.472 16.298 5.077 22.383-1.008l47.27-47.27c6.904-6.904 6.412-18.205-.963-24.603C378.507 23.673 319.807 0 256 0 161.34 0 78.586 51.557 34.411 128.119l86.806 50.034c26.985-46.533 77.229-77.979 134.783-77.979z"
            fill="#ff4b26"
          />
          <path
            d="M354.932 135.693c6.643 5.472 16.299 5.077 22.383-1.008l47.27-47.27c6.903-6.904 6.411-18.205-.963-24.603C378.507 23.672 319.807 0 256 0v100.174c37.53 0 72.005 13.336 98.932 35.519z"
            fill="#d93f21"
          />
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>
