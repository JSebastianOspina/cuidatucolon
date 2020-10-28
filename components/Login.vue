<template>
  <div>
      <h3 class="text-center mt-6 text-4xl font-medium">Bienvenido</h3>

      <div class="text-center px-10">
          <form action="">
              <div class="mt-8">
                  <input class="py-3 px-5 w-full leading-tight shadow-md text-gray-700" type="email" name="email" id="email">
              </div>
               <div class="mt-10">
                  <input class="py-3 px-5 w-full shadow-md text-gray-700" type="password" name="contra" id="contra">
              </div>
              <p class="text-md font-light mt-6">
                ¿Olvidaste tu contraseña?
              </p>
                <button class="mt-6 py-3 rounded-full text-white bg-blue-900 px-7 w-full" type="submit">Iniciar sesión</button>
         <p class="text-md font-light mt-6 inline-block">
                ¿No tienes una cuenta?</p><a class="ml-1" href="">Regístrate</a>
          </form>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>