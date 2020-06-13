<template>
  <h1>About Page</h1>
  <h3>{{ title }}</h3>
  <NuxtLink to="/index">

  </NuxtLink>
</template>
<script>
export default {
  data () {
    return {
      title: 'About Us - Nuxt.js'
    }
  },
  head () {
    return {
      title: this.title,
      meta: [
        { hid: 'description', name: 'description', content: 'About our company Nuxt.js ' }
      ]
    }
  }
}
</script>
<style>
.container {
  text-align: center;
  margin-top: 150px;
  font-size: 20px;
}
</style>
