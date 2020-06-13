<template>
<div class="banner" id="banner">
  <div class="logo-and-title">
    <div class="title"><h6>This is Banner Page</h6></div>
  </div>
</div>
</template>

<script>
export default {
  name: 'banner'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Lobster&display=swap');
.logo-and-title {
  position: absolute;
  top: 0%;
  left: 30%;
  color: #f4bca2;
}
@media screen and (max-width: 1800px) {
  .logo-and-title {
    top: 20%;
  }
}
@media screen and (max-width: 1590px) {
  .logo-and-title {
    top: 20%;
    left: 10%;
  }
}
@media screen and (max-width: 1260px) {
  .logo-and-title {
    top: 20%;
    left: 5%;
  }
}
@media screen and (max-width: 1200px) {
  .logo-and-title {
    top: 20%;
    left: 5%;
  }
}
@media screen and (max-width: 800px) {
  .logo-and-title {
    top: 8%;
    left: 5%;
  }
}
.title {
  font-size: 10rem;
  font-family: 'Lobster', cursive;
}
@media screen and (max-width: 1200px) {
  .title {
    font-size: 8rem;
  }
}
@media screen and (max-width: 800px) {
  .title {
    font-size: 6rem;
  }
}
@media screen and (max-width: 420px) {
  .title {
    font-size: 2.5rem;
  }
}
@media screen and (max-width: 307px) {
  .title {
    font-size: 2rem;
  }
}
.subtitle {
  font-size: 2rem;
  margin-left: 10%;
  font-family: 'Roboto', sans-serif;
  font-style: italic;
}
@media screen and (max-width: 800px) {
  .subtitle {
    display: none;
  }
}
.img-fluid{
 height: 7rem;
 width: 100%;
}
</style>
