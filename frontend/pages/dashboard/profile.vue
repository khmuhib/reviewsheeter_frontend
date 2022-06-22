<template>
  <div>
    <div class="card">
      <div class="card-header">Profile</div>
      <div class="card-body">
        <form>
          <div class="form-group mb-3">
            <label for="">Your name </label>
            <input
              type="text"
              class="form-control"
              name="name"
              placeholder="Enter email"
            />
          </div>
          <div class="form-group mb-3">
            <label for="">Your email </label>
            <input
              type="text"
              class="form-control"
              name="email"
              placeholder="Enter email"
            />
            <has-error :form="registerForm" field="email"></has-error>
          </div>
          <div class="form-group mb-3">
            <label for="">Your Password</label>
            <input
              type="password"
              class="form-control"
              name="password"
              placeholder="Enter password"
            />
          </div>
          <div
            class="form-group d-flex justify-content-between align-items-center"
          >
            <button type="submit" class="btn btn-success">
              Update Profile
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "profile",
};
</script>

<style>
</style>
