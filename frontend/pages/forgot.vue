<template>
    <div class="row justify-content-center my-5">
        <div class="col-6">
            <div class="card">
                <div class="card-header">
                    Forgot Password
                </div>
                <div class="card-body">
                    <form>
                        <div class="form-group mb-3">
                            <label for="">Enter Email </label>
                            <input type="text" class="form-control" name="email" placeholder="Enter email">
                        </div>
                        <div class="form-group d-flex justify-content-between align-items-center">
                            <button type="submit" class="btn btn-success">
                                Send Password Reset Email
                            </button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'forgot'
}
</script>

<style>

</style>
