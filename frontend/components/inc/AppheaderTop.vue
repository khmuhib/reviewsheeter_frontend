<template>
  <div class="py-3 bg-warning">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <NuxtLink to="/"
            ><img src="/images/logo.png" alt="" class="header-top-logo-img"
          /></NuxtLink>
        </div>
        <div class="col-md-6 text-right">
          <a href="#">
            <img
              src="/images/header_top_ads.jpg"
              alt=""
              class="header-top-ads-img"
            />
          </a>
        </div>
        <div class="col-md-3 text-right d-flex align-items-center">
          <nuxt-link :to="{ name: 'login' }" class="btn btn-success m-2" v-if="!loggedIn">Login</nuxt-link>
          <nuxt-link :to="{ name: 'register' }" class="btn btn-primary m-2" v-if="!loggedIn">Sign up</nuxt-link>
          <nuxt-link :to="{ name: 'dashboard' }" class="btn btn-primary m-2" v-if="loggedIn">Dashboard</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

  computed: {
    loggedIn() {
      return this.$store.state.auth.loggedIn;
    },

  }
};
</script>

<style scoped>
</style>
