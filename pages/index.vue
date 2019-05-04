<template>
  <section class="container">
    <div>
      <h1 class="title">
        ♥ My Nuxt App ♥
      </h1>

      <nuxt-link
        to="/users/"
        class="button-link"
      >
        Users</nuxt-link>

      <button
        @click="navigateProgrammatically('/products')"
        class="button-link"
        >
          Products</button>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    navigateProgrammatically(page) {
      this.$router.push(page)
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #cc62c3;
  letter-spacing: 1px;
}

.button-link {
  border: 1px solid #cc62c3;
  background: transparent;
  padding: 10px 20px;
  text-decoration: none;
  color: #cc62c3;
  cursor: pointer;
}

.button-link:hover {
  text-decoration: none;
}
</style>
