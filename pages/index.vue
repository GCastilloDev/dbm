<template>
  <section>
    <Banner class="pb-16" />
    <OurServices id="services" class="mt-16 pb-16" />
    <AboutUs id="about-us" class="mt-16" />
    <Clients id="clients" class="my-16 py-16" />
    <Partners id="partners" class="mt-16 pt-16" />
  </section>
</template>

<script>
import Banner from "../components/Banner.vue";
import OurServices from "../components/OurServices.vue";
import AboutUs from "../components/AboutUs.vue";
import Clients from "../components/Clients.vue";
import Partners from "../components/Partners.vue";

export default {
  name: "IndexPage",
  components: {
    Banner,
    OurServices,
    AboutUs,
    Clients,
    Partners,
  },
};
</script>

<style>
.title__section {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 38px;
  line-height: 54px;
  color: #415364;
}

.title__section > span {
  border-bottom: solid 2px #ffdd3f;
}
</style>
