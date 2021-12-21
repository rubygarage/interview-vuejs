<template>
  <a-layout
    :style="{
      display: 'flex !important',
      flexDirection: 'column',
      minHeight: 'calc(100vh - 22px)',
    }"
    id="components-layout-demo-top"
    class="layout"
  >
    <Header />
    <Lists />
    <Footer />
  </a-layout>
</template>

<script>
import Header from "../stubs/Header.vue";
import Lists from "../stubs/Lists.vue";
import Footer from "../stubs/Footer.vue";

export default {
  name: "stubs",
  components: {
    Header,
    Lists,
    Footer,
  },
};
</script>
