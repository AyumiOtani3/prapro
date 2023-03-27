<template>
  <div class="hello">
    <Marquee />
    <h1>{{ msg }}</h1>
    <p>
      映画情報はこちら
      <a href="#" target="_blank" rel="noopener">Movie Museum</a>.
    </p>
    <h3>My Favourits</h3>
    <ul>
      <li><a href="#" target="_blank" rel="noopener">babel</a></li>
    </ul>
    <h3>Storys</h3>
    <ul>
      <li><a href="#" target="_blank" rel="noopener">Core Docs</a></li>
    </ul>
    <h3>Movie Subscription</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
    </ul>
  </div>
</template>

<script>
import Marquee from './Marquee.vue';

export default {
  name: 'HelloWorld',
  components: {
    Marquee
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
