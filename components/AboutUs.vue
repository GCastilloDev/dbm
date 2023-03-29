<template>
  <section class="about-us">
    <v-container class="d-flex justify-center pt-15 pb-14">
      <section class="about-us__container d-flex">
        <figure v-if="this.$vuetify.breakpoint.mdAndUp">
          <img src="~/static/about_us.png" width="100%" alt="" />
        </figure>
        <div>
          <h2 class="title__section"><span>NOSO</span>TROS</h2>
          <p v-if="this.$vuetify.breakpoint.smAndDown">
            <img src="~/static/about_us-2.png" width="100%" alt="" />
          </p>
          <p>
            Somos una
            <span
              >compañía especialista en el desarrollo de comercio
              electrónico</span
            >, brindamos asesoría a nuestros clientes nacionales e
            internacionales para la creación de una sociedad mercantil lista
            para la venta en plataformas digitales de comercio en línea, con el
            soporte y acompañamiento profesional tanto en el área de comercio
            electrónico y jurídico.
          </p>
          <p>
            Con nuestros servicios <span>ahorrarás tiempo y dinero</span>, ya
            que no tendrás que experimentar la etapa de aprendizaje en el uso de
            las plataformas electrónicas, optimizando tiempos y productos.
          </p>
        </div>
      </section>
    </v-container>
  </section>
</template>

<script>
export default {
  name: "AboutUs",
};
</script>

<style lang="css" scoped>
.about-us__container {
  width: 80%;
}

figure {
  width: 100vw;
  margin-right: 3rem;
}

.about-us {
  background-color: #97afb2;
}

.title__section {
  color: #ffffff;
  margin-bottom: 1.5rem;
}

p {
  font-family: "Karla";
  font-style: normal;
  font-weight: 500;
  line-height: 26px;
  color: #ffffff;
}

p > span {
  font-weight: 700;
  color: #ffdd3f;
}

@media only screen and (max-width: 959px) {
  .about-us__container {
    width: 100%;
  }
}
</style>