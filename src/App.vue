<script setup>
import { ref } from "vue";
import Header from "./components/Header.vue";
import MainHeader from "./components/MainHeader.vue";
import Services from "./components/Services.vue";
import Business from "./components/Business.vue";
import Team from "./components/Team.vue";
import Review from "./components/Review.vue";
import Footer from "./components/Footer.vue";



</script>

<template>
  <Header />
  <main class="Main">
    <MainHeader />
    <Services />
    <Business />
    <Team />
    <Review />
  </main>
  <Footer />
</template>

<style scoped>
.Main {
  min-height: 100vh;
  height: auto;
  margin: 0 auto;

  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>
