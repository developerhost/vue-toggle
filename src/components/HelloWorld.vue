<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2 v-show="showText">{{ text }}</h2>
    <!--https://i.gyazo.com/4be26312187ef5c44fd6af033e077d3b.png-->
    <button v-on:click="toggle">toggle</button>
    <!-- https://gyazo.com/a953a7b4e7b1cf083ee208c05a1f83eb -->
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      text: 'Test data',
      showText: false
    }
  },
  methods: {
    toggle: function () {
      this.showText = !this.showText
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
</style>
