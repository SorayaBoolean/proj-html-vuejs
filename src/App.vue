<template>
  <div>
    <MyHeader/>
    <MyMain/>
    <MyFooter/>

  </div>
    
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'



export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  }
}
</script>

<style lang="scss">
  
  @import '~@fortawesome/fontawesome-free/css/all.css';

 *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
</style>
