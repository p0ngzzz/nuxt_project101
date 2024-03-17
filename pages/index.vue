<template>
  <div>
    <h1>Nuxt JS Tutorial</h1>
    <br>
    <button class="btn">
      <nuxt-link to="/about"><h3>About</h3></nuxt-link>
    </button>
    <button class="btn">
      <nuxt-link to="/users"><h3>Users</h3></nuxt-link>
    </button>
    <button class="btn">
      <nuxt-link to="/products"><h3>Products</h3></nuxt-link>
    </button>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  layout: 'default'
}
</script>

<style>
/* .btn {
  border: 2px solid black;
  padding: 20px;
  background: #000;
  box-shadow: 3px 3px 3px #343434;
  
}
.btn h3 {
  color: #fff;
  transition: all 0.5s linear;

}
.btn:hover h3 {
  color: #dba717;
  font-size: 20px;
}
.nuxt-link-exact-active {
  text-decoration: none;
} */
</style>
