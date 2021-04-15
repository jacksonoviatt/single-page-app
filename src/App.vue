<template>
  <div id="app">
    <page-header></page-header>
    <page-body></page-body>

    <page-footer></page-footer>
   
  </div>
</template>

<script>
// here we import the components we created
import PageBody from './components/PageBody.vue'
import PageFooter from './components/PageFooter.vue'
import PageHeader from './components/PageHeader.vue'


export default {
  name: 'App',
  // state the components in this object
  components: {
    PageBody,
    PageHeader,
    PageFooter

  }
}
</script>

<style>
body {
  background-color: #1F2F16;
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #FACFAD;
}

</style>
