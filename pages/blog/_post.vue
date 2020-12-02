<template>
  <div class="px-3 blog">
    <TarjetaTitulo titulo ="5 tipos de influencers y 7 maneras de hacer marketing con ellos [GUÍA]"/>
    <!---
    <div class="post-content mt-4">
      <p>
        El marketing de influencers está de moda. Los negocios cada vez lo
        tienen más en cuenta y lo piden a las agencias porque da buenísimos
        resultados.
      </p>
      <p>
        En la VI edición de <a href="">ProMarketingDay</a>, le dedicamos un
        espacio especial a estas nuevas estrellas de la comunicación y a las
        marcas que están implicándolos en sus estrategias de marketing.
      </p>
      <h2 class="">Qué es un influencer (H2)</h2>
      <p>
        El marketing de influencia tiene un claro protagonista: el influencer. Y
        no importa si es famoso o no, lo importante es que sea capaz de generar
        conversiones.
      </p>
      <h3 class="">Tipos de influencer (H3)</h3>
      <p>
        No siempre las llamadas celebrities o famosos consiguen generar este
        engagement. Es frecuente que descuiden a su comunidad o no se preocupan
        en generar contenido útil para sus seguidores, lo cual termina por
        afectar su credibilidad como influencer.
      </p>
      <div class="text-justify mb-3">
        <h3>¿Te ha sido útil?</h3>
        <h2>¡Comparte este artículo en tus redes sociales</h2>
      </div>
    </div>
    -->
    <div class="post-content mt-4">
      <pre>
        {{articulo}}
      </pre>

    </div>

    <Facebook class="mb-2" />
    <Twitter class="mb-2" />
    <Whatsapp class="mb-2" />
  </div>
</template>
<script>
export default {
  layout: "blog",
  async asyncData({ $content,params }) {
    const articulo = await $content('blog/'+params.post || "index").fetch();
    return { articulo };
  },
};
</script>
<style >
.blog {
  font-family: "Muli";
  font-weight: 300;
}
.post-content {
  text-align: justify;
  font-size: 20px;
}
.post-content p {
  color: #444;
  margin-bottom: 7px;
}
.post-content a {
  color: #1cbacc;
}
.post-content h2 {
  font-size: 1.875em;
  font-weight: 200;
  text-align: center;
  margin-bottom: 7px;
}
.post-content h3 {
  font-size: 1.775em;
  font-weight: 200;
  text-align: center;
  margin-bottom: 7px;
}
</style>