<template>
  <div id="app">
    <headerTest/>
  </div>
</template>

<script>
import headerTest from './components/header';

export default {
  name: 'app',
  components: {
    headerTest
  },
}
</script>

<style lang="scss">
#app {
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
	}
</style>
