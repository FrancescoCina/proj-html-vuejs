<template>
  <div id="app">
    <Header :links="links"></Header>
    <Main :pricingInfos="pricingInfos"></Main>
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
      pricingInfos: [
        {
          service: "Designing",
          forWho: "PROCESS",
          price: 40,
          detailOne: "Creative Design Enabled",
          detailTwo: "Vibrant Color Usage",
          detailThree: "Eye Catching Design",
          detailFour: "Extreme Typography",
          detailFive: "Exceptional Design",
          backgroundClass: "",
          backgroundButton: "pink-button",
        },
        {
          service: "Developing",
          forWho: "PRODUCT",
          price: 60,
          detailOne: "Creative Design Enabled",
          detailTwo: "Vibrant Color Usage",
          detailThree: "Eye Catching Design",
          detailFour: "Extreme Typography",
          detailFive: "Exceptional Design",
          backgroundClass: "pink-card",
          backgroundButton: "white-back",
        },
        {
          service: "Supporting",
          forWho: "CLIENTS",
          price: 80,
          detailOne: "Creative Design Enabled",
          detailTwo: "Vibrant Color Usage",
          detailThree: "Eye Catching Design",
          detailFour: "Extreme Typography",
          detailFive: "Exceptional Design",
          backgroundClass: "",
          backgroundButton: "pink-button",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "assets/scss/style.scss";
</style>
