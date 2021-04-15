<template>
  <div class="hello">
    <section>
    <fun-fact-list></fun-fact-list>
    <chickadee-video></chickadee-video>
    
    </section>
    <section>
      <attrack-chickadee></attrack-chickadee>
    </section>
  </div>
</template>

<script>
// here we import the components we created 
// Don't forget to use proper casing
import AttrackChickadee from './AttrackChickadee.vue'
import ChickadeeVideo from './ChickadeeVideo.vue'
import FunFactList from './FunFactList.vue'
export default {
  //  name of the component we are in
  name: 'PageBody',
  // names of the components nested within this component
  components: {
    FunFactList,
    ChickadeeVideo,
    AttrackChickadee,
  }
}

</script>


<style scoped>
.hello {
  background:  #1F2F16 url("../assets/chickadeeGreenBackdrop.jpeg");
  background-position: center;
  background-repeat: no-repeat;
  height: 100vh;
  width: 100vw;
  position: absolute;
  top: 100px;
  display: grid;
  grid-template-columns: 3fr 2fr;
}

section {
  width: 800px;
  padding: 10px;
  margin-left: -70px;
  display: grid;
  justify-items: center;
  padding-bottom: 50px;
}

</style>
