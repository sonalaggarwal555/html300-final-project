<template>
<div id="app">
<!--Place photos component on images page-->
  <section v-if="images" class="flex-container">
    <photos
      v-for="image in images"
      :image="image"
      :key="image.src"
      />
  </section>
</div>
</template>

<script>
import photos from './photos.vue';
import mixins from './mixins';
//Create variable paths for images
var card1 = require('../static/cover.JPG');
var card2 = require('../static/cover2.jpg');
var card3 = require('../static/flowercocktails.jpg');
var card4 = require('../static/lemonade.jpg');
var card5 = require('../static/pic-14.jpg');
var card6 = require('../static/pic-13.jpg')
//Images object and data
export default {
name: 'Images',
mixins: [mixins],
components: {
  photos
},
data () {
  return {
    images: [
      { src: card1, alt: 'Sunset View', name: 'Classic Red', caption: 'this classic is the quint essential sign of spring.' },
      { src: card2, alt: 'Red trees', name: 'Fire on the Mountain', caption: 'With petals that look like flames, this variety is only for the bold.' },
      { src: card3, alt: 'Violet cocktails', name: 'Amethyst', caption: 'If you love a splash of purple, this one is perfect for your home or as a gift.' },
      { src: card4, alt: 'Lemonades', name: 'Peach Sunrise', caption: 'makes an appearance every few years.' },
      { src: card5, alt: 'bright cocktail', name: 'Scarlett Letter', caption: 'This head-turner is great and vibrant pop of color.' },
      { src: card6, alt: 'watermelon cocktail', name: 'Snow Top', caption: 'This elegent and clean variety can brighten up your party.' }
    ]
  }
 }
}
</script>

<style scoped>
button {
  margin:3rem;
  color: #e4cece;
  border-style: solid;
  background-color: white;
  position: relative;
}
.flex-container {
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-start;
  align-content: space-around;
  justify-content: center;
  margin: 3rem;
}
.caption {
  padding: 1rem;
}
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
