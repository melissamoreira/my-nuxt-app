<template>
    <section class="container">
        <div>
            <input
                v-model="userId"
                type="text"
            />

            <button @click="onLoadUser">Load User</button>
        </div>

        <nuxt-link to="/">< Back Home</nuxt-link>
    </section>
</template>

<script>
export default {
    data: () => ({
        userId: ''
    }),

    methods: {
        onLoadUser () {
            this.$router.push('/users/' + this.userId)
        }
    }
}
</script>
<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
