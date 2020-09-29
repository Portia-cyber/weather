<template>
  <div id="app" class="container mx-auto">
    <weather></weather>
  </div>
</template>

<script>
import Weather from './components/weather.vue'

export default {
  name: 'App',
  components: {
    Weather
  }
}
</script>

<style lang="scss">
#app {
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}
body{
  font-family: "Roboto Light",serif;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app.warm{
  background-image: url("./assets/warm-bg.jpg");
}
</style>
