<template>
  <div class="flex flex-col w-screen h-screen">
    <div class="imagen relative">
      <div class="custom-shape-divider-top-1603949195">
        <svg
          data-name="Layer 1"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 1200 120"
          preserveAspectRatio="none"
        >
          <path
            d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z"
            opacity=".5"
            class="shape-fill"
          ></path>
          <path
            d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z"
            class="shape-fill"
          ></path>
        </svg>
      </div>
      <div
        class="w-10 h-10 shadow-xl flex rounded-full bg-white absolute"
        style="top: 10px; left: 10px"
      >
          <div class="text-center mt-1 flex w-full h-full">
              <svg
                xmlns="http://www.w3.org/2000/svg"
              class=""
              >
                <defs>
                  <filter
                    id="a"
                    x="0"
                    y="0"
                    width="35.873"
                    height="35.42"
                    filterUnits="userSpaceOnUse"
                  >
                    <feOffset dy="3" />
                    <feGaussianBlur stdDeviation="3" result="blur" />
                    <feFlood flood-color="#fff" flood-opacity=".588" />
                    <feComposite operator="in" in2="blur" />
                    <feComposite in="SourceGraphic" />
                  </filter>
                </defs>
                <g filter="url(#a)">
                  <path
                    data-name="arrow-right-solid"
                    d="M19.274 7.167l-.886-.886a.953.953 0 00-1.352 0l-7.755 7.751a.953.953 0 000 1.352l7.755 7.755a.953.953 0 001.352 0l.886-.886a.958.958 0 00-.016-1.368l-4.807-4.579h11.464a.955.955 0 00.958-.956v-1.278a.955.955 0 00-.957-.957H14.451l4.807-4.579a.952.952 0 00.016-1.369z"
                    fill="#404040"
                  />
                </g>
              </svg>
          </div>
      </div>
      <img
        :src="data.image"
        class="redondo w-full h-64 object-cover"
        :alt="data.nombre"
      />
    </div>
    <div class="info text-center mt-2 mx-4">
      <h1 class="font-bold text-xl">
        {{ data.nombre }}
      </h1>
      <p class="text-xs mt-2">
        {{ data.descripcion }}
      </p>
    </div>
    <div
      class="info sombra-pequena flex flex-col rounded-xl bg-white py-4 mt-3 px-1 mx-4"
    >
      <div>
        <p class="text-sm text-center">Información nutricional</p>
      </div>
      <div class="flex justify-around mt-2">
        <div>
          <p class="text-sm text-center text-red-500 font-bold">600</p>
          <p class="text-xs text-center">calorias</p>
        </div>
        <div>
          <p class="text-sm text-center font-bold">2,8g</p>
          <p class="text-xs text-center">grasas</p>
        </div>
        <div>
          <p class="text-sm text-center font-bold">45,7g</p>
          <p class="text-xs text-center">carbohidratos</p>
        </div>
        <div>
          <p class="text-sm text-center font-bold">9,8g</p>
          <p class="text-xs text-center">proteina</p>
        </div>
      </div>
    </div>
    <div
      class="ingredientes sombra-pequena flex flex-col bg-white rounded-xl p-5 px-5 mx-4 mt-3"
    >
      <div>
        <p class="text-sm text-center font-bold">Ingredientes</p>
      </div>
      <div class="flex justify-around mt-3">
        <div class="flex flex-col items-center">
          <img
            class="w-10 h-10 rounded-full"
            :src="data.image"
            :alt="data.nombre"
          />
          <p class="text-xs">Cerezas</p>
        </div>
        <div class="flex flex-col items-center">
          <img
            class="w-10 h-10 rounded-full"
            :src="data.image"
            :alt="data.nombre"
          />
          <p class="text-xs text-center">Cerezas</p>
        </div>
        <div class="flex flex-col items-center">
          <img
            class="w-10 h-10 rounded-full"
            :src="data.image"
            :alt="data.nombre"
          />
          <p class="text-xs text-center">Cerezas</p>
        </div>
        <div class="flex flex-col items-center">
          <img
            class="w-10 h-10 rounded-full"
            :src="data.image"
            :alt="data.nombre"
          />
          <p class="text-xs text-center">Cerezas</p>
        </div>
      </div>
    </div>
    <div
      class="preparacion sombra-pequena flex flex-col bg-white rounded-xl p-5 px-5 mx-4 mt-3 mb-2"
    >
      <div>
        <p class="text-sm text-center font-bold">Preparacion</p>
      </div>
      <div class="flex flex-col">
        <ul>
          <li>Paso 1</li>
          <li>paso 2</li>
          <li>paso 3</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ params }) {
    const slug = params.receta; // When calling /abc the slug will be "abc"
    return { slug };
  },
  layout: "insideapp",
  data() {
    return {
      data: {
        nombre: "Arroz con verduras",
        image: "https://images.unsplash.com/photo-1519996409144-56c88c9aa612",
        descripcion: "Arroz mixto con verduras al vapor. Ideal para domingo",
      },
    };
  },

  head() {
    return {
      title: this.slug,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Receta de " + this.slug,
        },
        {
          hid: "og:description",
          name: "og:description",
          content: "Receta de " + this.slug,
        },
      ],
    };
  },
};
</script>

<style>
.redondo {
  border-bottom-right-radius: 3rem;
  border-bottom-left-radius: 3rem;
}
.flecha{
     position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
}
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
  fill: #6cc57c;
}

/** For mobile devices **/
@media (max-width: 767px) {
  .custom-shape-divider-bottom-1603949143 svg {
    width: calc(100% + 1.3px);
    height: 54px;
  }
}
</style>