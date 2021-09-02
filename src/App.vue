<template>
  <div>
    <Header/>
    <Main/>
    <Review/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Review
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

:root{
  --main-color: #D2691E;

  --logo-font: 'Oleo Script Swash Caps', cursive;
}

*, *::before, *::after{
  box-sizing: inherit;
}

html{
  box-sizing: border-box;
  font-size: 62.5%; /*1rem === 10px*/
}

body{
  margin: 0;
}

.btn{
  color: #fff;
  background-color: var(--main-color);
  border-radius: 5px;
  border: none;
  padding: 1rem 1.5rem;
  cursor: pointer;
}
</style>
