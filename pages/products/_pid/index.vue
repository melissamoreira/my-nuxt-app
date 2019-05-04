<template>
    <section class="container">
        <h1 class="title">Product <span>{{ $route.params.pid }}</span></h1>

        <nuxt-link to="/products">< Back to Products</nuxt-link>
    </section>
</template>

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

.title span {
    text-transform: capitalize;
}
</style>
