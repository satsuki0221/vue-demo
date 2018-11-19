<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App">
      <Test>
        {{ count }}
      </Test>
      <Test>
        {{ count }}
      </Test>
      <Test>
        {{ count }}
      </Test>
      <Testn :count="count"></Testn>
    </HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Test from './components/Test.vue';
import Testn from './components/Testn.vue';


export default {
  name: 'app',
  data: function () {
    return {
      count: 0
    }
  },
  components: {
    HelloWorld,
    Test,
    Testn
  },
  mounted: function () {
    var _this = this;
    setInterval(() => {
      _this.count++
    }, 1000)
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
