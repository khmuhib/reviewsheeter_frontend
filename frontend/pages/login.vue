
<template>
    <div class="row justify-content-center my-5">
        <div class="col-6">
            <div class="card">
                <div class="card-header">
                    Login Page
                </div>
                <div class="card-body">
                    <form>
                        <div class="form-group mb-3">
                            <label for="">Enter Email </label>
                            <input type="text" class="form-control" name="email" placeholder="Enter email">

                        </div>
                        <div class="form-group mb-3">
                            <label for="">Enter Password</label>
                            <input type="password" class="form-control" name="passwrd" placeholder="Enter password">

                        </div>
                        <div class="form-group d-flex justify-content-between align-items-center">
                            <button type="submit" class="btn btn-success">Give me Access</button>
                            <nuxt-link :to="{ name: 'register' }">Don't have account?</nuxt-link>
                        </div>
                        <div class="mt-3">
                            <nuxt-link :to="{ name: 'forgot' }">Forgot Password? </nuxt-link>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'login'


}
</script>

<style>
</style>
