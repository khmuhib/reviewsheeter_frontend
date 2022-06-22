<template>
  <div class="container">
    <div class="row my-3">
      <div class="col-3">
        <div class="card">
          <div class="card-header">Deshboard</div>
          <div class="card-body">
            <ul>
              <li>
                <nuxt-link :to="{ name: 'dashboard' }">Dashboard</nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{ name: 'dashboard-profile' }"
                  >Profile</nuxt-link
                >
              </li>
              <li><a href="#" @click.prevent="logout">Logout</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-9">
        <nuxt-child />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "deshboard",
  middleware: 'auth',
  methods: {
    async logout() {
      await this.$auth.logout()
    }
  },
};
</script>

<style>
</style>
