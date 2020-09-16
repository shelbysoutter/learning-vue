<template>
  <div id="app">
    <Header />
    <SearchMovies />
    <Movies v-bind:movies="movies"/>
  </div>
</template>

<script>
import Header from './components/layout/Header';
import Movies from './components/Movies';
import SearchMovies from './components/SearchMovies';

export default {
  name: 'App',
  components: {
    Header,
    Movies,
    SearchMovies
  },
  data() {
    return {
      movies: [
        {
          id: 1,
          title: "Movie One"
        },
        {
          id: 2,
          title: "Movie Two"
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
