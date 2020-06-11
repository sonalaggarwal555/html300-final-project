<template>
  <div id="app">
    <header>
      <banner />
    </header>
    <!--Bootstrap responsive navbar with router-->
   <nav class="navbar navbar-expand-lg m-3">
     <a class="navbar-brand" href="#"><strong>Welcome</strong></a>
     <nav class="navbar-nav">
       <nuxt-link to="/HelloWorld" class="nav-item nav-link active">Home <span class="sr-only">(current)</span></nuxt-link>
       <nuxt-link to="/images" class="nav-item nav-link">Images</nuxt-link>
       <nuxt-link to="/grid" class="nav-item nav-link">Grid</nuxt-link>
       <nuxt-link to="/accordian" class="nav-item nav-link">Accordian</nuxt-link>
     </nav>
   </nav>

   <nuxt/>

   <div class="end"></div>
    <!--Basic footer-->
    <footer class="footer">
        <p>This is footer</p>
    </footer>
  </div>
</template>
<script>
import banner from '../pages/banner.vue';
export default {
  name: 'App',
  components: {
    banner
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');
header {
  margin:0 10rem 0 10rem;
}
.navbar {
  background-color: #F6F1EE;
  font-family: 'Roboto', sans-serif;
  border-style: solid;
  border-size: 0.3rem;
  border-color: #FBDCCE;
}
.navbar a {
  color: #EFA885;
}
.footer {
    color: black;
    background-color: #F6F1EE;
    margin-top: 2rem;
    padding: 1rem;
    text-align: center;
    font-family: 'Roboto', sans-serif;
}
.end {
  clear: both;
}
</style>
