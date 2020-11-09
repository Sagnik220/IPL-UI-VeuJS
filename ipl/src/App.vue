<template>
  <div id="app">
    <header>
      <Navbar />
    </header>
    <p><img src="./assets/ipl.jpg" width="1950" height="1000" /></p>
  </div>
</template>

<script>
import Navbar from './components/Navbar';
export default {
  name: 'app',
  components: {
    Navbar
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'montserrat', sans-serif;
}
header {
  width: 100vw;
  background-color: #222;
  padding: 15px;
}
</style>