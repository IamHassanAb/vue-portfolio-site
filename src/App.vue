<template>
  <div id="app">
    <Header></Header>
    <!-- <section class="section" id="home" key="home">
      <Home />
    </section> -->
    <section class="section" id="about" key="about">
      <About />
    </section>
    <section class="section" id="projects" key="projects">
      <Projects />
    </section>
    <section class="section" id="contact" key="contact">
      <Contact />
    </section>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import About from './components/About.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';

export default {
  name: 'App',
  components: {
    Header,
    About,
    Projects,
    Contact
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}

.section {
  padding: 20px;
  margin: 20px;
  border-radius: 20px;
  box-shadow: 8px 8px 16px #d1d9e6, -8px -8px 16px #ffffff;
}
</style>