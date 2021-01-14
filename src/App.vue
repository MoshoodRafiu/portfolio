<template>
  <div id="app">
    <app-header/>
    <app-about/>
    <app-projects/>
    <app-contact/>
  </div>
</template>

<script>
import Header from './components/Header';
import About from './components/About';
import Projects from './components/Projects';
import Contact from './components/Contact';

export default {
  name: 'App',
  components: {
    appHeader: Header,
    appAbout: About,
    appProjects: Projects,
    appContact: Contact
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@100;300;400;500&display=swap');
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
  .col-lg-4{
    padding-right: 40px;
    padding-left: 40px;
  }
  @media screen and (max-width: 600px) {
      .col-lg-4{
        padding-right: 20px;
        padding-left: 20px;
      }
  }
</style>
