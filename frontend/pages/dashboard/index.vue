<template>
  <div>
    <div class="card">
      <div class="card-header">Dashboard</div>
      <div class="card-body">
        <h4 v-if="loggedIn">Welcome, {{user.name}}</h4>
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptates
          eveniet obcaecati totam quod iure eligendi?
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "index",
  computed: {
    loggedIn () {
      return this.$store.state.auth.loggedIn
    },
    user () {
      return this.$store.state.auth.user
    }
  }
};
</script>

<style>
</style>
