<template>
  <div>
    <HomeSlider></HomeSlider>
    <CallToAction></CallToAction>
    <Hero />




  </div>
</template>

<script>
import Hero from './Hero.vue';
import CallToAction from './CallToAction.vue';
export default {
  name: "home",
  components: { Hero, CallToAction }
};
</script>

<style>
</style>
