<template>
  <div id="app">
    <tabs :currentIndex="currentIndex" @onIndex="getCurrentIndex" >
      <tab  index="1" >
        <div>内容1</div>
      </tab>
      <tab label="tab2" index="2" >
        <div>内容2</div>
      </tab>
      <tab label="tab3" index="3" >
        <div>内容3</div>
      </tab>
    </tabs>
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      currentIndex:1
    }
  },
  methods:{
    getCurrentIndex(index){
      this.currentIndex = index;
    }
  },
  components: {
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
