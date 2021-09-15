<template>
  <div id="app">
    <Header :links="links"></Header>
    <Main></Main>
    <Footer :links="links"></Footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      links: [
        {
          name: "Home",
          url: "#",
        },
        {
          name: "About",
          url: "#",
        },
        {
          name: "Services",
          url: "#",
        },
        {
          name: "Blog",
          url: "#",
        },
        {
          name: "Contact",
          url: "#",
        },
        {
          name: "Portfolio",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "assets/scss/style.scss";
</style>
