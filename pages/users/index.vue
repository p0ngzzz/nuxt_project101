<template>
  <div id="users-page">
    <ul>
        <li v-for="user in 10" :key="user">
            UserID: <nuxt-link :to="`/users/${user}`">{{ user }}</nuxt-link>
        </li>
    </ul>
    <button class="btn">
      <nuxt-link to="/"><h3>Back to Home</h3></nuxt-link>
    </button>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>