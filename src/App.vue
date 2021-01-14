<template>
  <div id="app">
    <app-header/>
    <app-about/>
  </div>
</template>

<script>
import Header from './components/Header';
import About from './components/About';

export default {
  name: 'App',
  components: {
    appHeader: Header,
    appAbout: About
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Odibee+Sans&display=swap');
  body{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: 'Odibee Sans', cursive;
  }
</style>
