<template>
  <div>
    <Header />
    <Welcome />
    <Credentials />
    <Skills />
    <Projects />
    <Contacts />
  </div>

</template>

<script>
import Header from './components/Header'
import Welcome from './components/Welcome'
import Credentials from './components/Credentials'
import Skills from './components/Skills'
import Projects from './components/Projects'
import Contacts from './components/Contacts'
export default {
  name: 'App',
  components: {
    Header,
    Welcome,
    Credentials,
    Skills,
    Projects,
    Contacts
  }
}
</script>

<style>
#app {
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  color: #F0EBF4
}

.title-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.title-page {
  text-align: center;
  margin: 2rem auto;
  font-size: 2.4em;
  text-decoration: underline;
}

@media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
  * {
    font-size: 100%;
  }
}

</style>
