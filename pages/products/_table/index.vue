<template>
  <div class="table-page">
    <h1>Table {{ id }}</h1>
    <ul>
      <li v-for="product in 10" :key="product">
        <!-- <h3>Product: <nuxt-link :to="`/products/${table}/${product}`">{{ product }}</nuxt-link></h3> -->
        <h3>
          Product:
          <nuxt-link
            :to="{
              path: `/products/${id}/${product}`,
              params: [{ table: `${id}` }, { id: `${product}` }],
            }"
            >{{ product }}</nuxt-link
          >
        </h3>
      </li>
    </ul>
    <button class="btn">
      <nuxt-link to="/products"><h3>Back to Products</h3></nuxt-link>
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: this.$route.params.table,
    }
  },
  mounted() {
    console.log(this.$route)
  },
}
</script>

<style></style>
