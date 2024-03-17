<template>
  <div id="product">

    <h3>Table: {{table}} Product: {{ id }}</h3>
    <button class="btn">
      <nuxt-link :to="`/products/${table}/`"><h3>Back to Table{{ table }}</h3></nuxt-link>
    </button>
    <!-- {{ $route }} -->
  </div>
</template>

<script>
export default {
  name: "Product",
  data() {
    return {
      id: this.$route.params.id,
      table: this.$route.params.table
    }
  },
  mounted() {
    console.log(this.$route)
    // console.log(this.$route.params.id)
    // console.log(this.$route.params.table)
  },
}
</script>

<style>

</style>