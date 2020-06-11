<template>
    <div class="faq-container">
        <h2 class="m-3">Frequently asked questions</h2>
        <!--Use v-for to populate accordion-->
        <div v-for="item in items" class="accordion" id="accordion">
            <div class="card">
              <div class="card-header" id="headingOne">
                <h2>
                  <button class="btn btn-link" type="button" v-on:click="show = !show" data-target="#collapseOne">
                    {{ item.faq }}
                  </button>
                </h2>
              </div>
              <div id="collapseOne" v-if="show" class="collapse show" data-parent="#accordion">
                <div class="card-body">
                    {{ item.answer }}
                </div>
              </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
name: 'Images',
data () {
  return {
  items: [
    { faq: 'Whats the purpose and usage?', answer: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' },
    { faq: 'Origins and Discovery?', answer: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' },
    { faq: 'Where should I plant my bulbs?', answer: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' },
    { faq: 'How long do they last?', answer: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' },
    { faq: 'What sets them above the rest?', answer: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' },
  ],
  show: false,
  }
}
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Lobster&display=swap');
.faq-container {
  margin: 3rem;
}
h2 {
  font-family: 'Roboto', sans-serif;
}
.btn {
  color: #E7C9B1;
  font-family: 'Roboto', sans-serif;
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
