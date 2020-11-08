<template>
  <div id="app">
    <header>
      <Navbar/>
    </header>
  </div>
</template>

<script>
import Navbar from './components/Navbar'

export default {
  name: 'App',
  components: {
      Navbar
  }
}
</script>

<style>
* {
    box-sizing: border-box;
    margin:0;
    padding:0;
}
body{
  font-family: 'monstserrat', sans-serif;
}

header{
  width: 100ww;
  background-color:#222;
  padding:15px;
}
</style>
