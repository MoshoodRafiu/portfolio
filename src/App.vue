<template>
  <div id="app">
    <app-header/>
    <app-about/>
    <app-projects/>
  </div>
</template>

<script>
import Header from './components/Header';
import About from './components/About';
import Projects from './components/Projects';

export default {
  name: 'App',
  components: {
    appHeader: Header,
    appAbout: About,
    appProjects: Projects
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
  button:focus{
    outline: none;
  }
</style>
