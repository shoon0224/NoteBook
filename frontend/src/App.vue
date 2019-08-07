<template>
  <div id="app">
    <Nav/>
    <router-view/>
  </div>
</template>

<script>
import{
  Nav
} from './components/Components'
export default {
  name: 'App',
  components: {
    Nav
  }
}
</script>

<style>
body {
     background-color: black;/*#0F1A31*/
    }
</style>
