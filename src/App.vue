<template>
  <div id="app">
    <OverallResults/>
    <LatestResults/>
    <Racers/>
  </div>
</template>

<script>
import OverallResults from './components/OverallResults';
import LatestResults from './components/LatestResults';
import Racers from './components/Racers';

export default {
  name: 'App',
  components: {
    OverallResults,
    LatestResults,
    Racers,
  },
};
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
