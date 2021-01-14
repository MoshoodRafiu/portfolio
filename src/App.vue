<template>
  <div id="app">
    <app-header/>
  </div>
</template>

<script>
import Header from './components/header/Header';

export default {
  name: 'App',
  components: {
    appHeader: Header
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
