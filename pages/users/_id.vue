<template>
  <div id="user">
    <h1>UserID:  {{ $route.params.id }}</h1>
    <button class="btn">
      <nuxt-link to="/users"><h3>Back to Users</h3></nuxt-link>
    </button>

  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>