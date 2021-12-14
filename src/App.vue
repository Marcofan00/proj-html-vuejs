<template>
  <div id="app">
    <Myheader />
    <Mymain />
    <Myfooter />
  </div>
</template>
<script>
import Myheader from './components/Myheader.vue'
import Mymain from './components/Mymain.vue'
import Myfooter from './components/Myfooter.vue'
export default {
  name: 'App',
  components: {
    Myheader,
    Mymain,
    Myfooter
  }
}
</script>

<style lang="scss">
   *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    } 
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@900&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');
</style>

