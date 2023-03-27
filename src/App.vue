<template>
  <div id="app">
    <Header />
    <HelloWorld msg="映画情報集めたい" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Marquee from './components/Marquee.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Header,
    // eslint-disable-next-line vue/no-unused-components
    Marquee
  },
  data() {
    return {
      movies: [] // API から取得した映画情報を格納する配列
    }
  },
  mounted() {
    // TMDb API を呼び出す処理
    const apiKey = 'YOUR_API_KEY_HERE'
    const apiUrl = `https://api.themoviedb.org/3/movie/popular?api_key=${apiKey}&language=ja-JP`

    fetch(apiUrl)
      .then(response => response.json())
      .then(data => {
        this.movies = data.results // 取得した映画情報を配列に格納する
      })
      .catch(error => console.error(error))
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: pink;
  margin-top: 60px;
}
</style>
