<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        Assignment 09
      </h1>
      <h2 class="subtitle">
        Final project for html300
      </h2>
      <div class="links">
      <ul>
        <li><nuxt-link to="/HelloWorld">Helloworld </nuxt-link></li>
        <li><nuxt-link to="/Accordian">Accordian</nuxt-link></li>
        <li><nuxt-link to="/images">Images</nuxt-link></li>
        <li><nuxt-link to="/grid">Grid</nuxt-link></li>
      </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
export default {
  components: {
    Logo
  }
}
</script>

<style>
ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
