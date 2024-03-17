<template>
  <div>
    <h1>Table of Products</h1>
    <ul>
        <li v-for="(table,index) in 7" :key="index">
            <h2>Table: <nuxt-link :to="`/products/${table}`">{{ table }}</nuxt-link></h2>
        </li>
    </ul>
    <button class="btn">
      <nuxt-link to="/"><h3>Back to Homepage</h3></nuxt-link>
    </button>
  </div>
</template>

<script>
export default {
  name: "Products",
  mounted() {
    console.log(this.$route)
  },
}
</script>

<style>

</style>