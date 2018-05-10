<template>
  <div id="app">
    <Nav />
    <!-- <img src="./assets/logo.png"> -->
    <Home/>

    <footer class="footer">
      <div class="container">
        <div class="columns">
          <div class="column">
            <p>made <i class="fa fa-heart"></i> by ismael Garcia </p>
          </div>
          <div class="column has-text-rigth">
            <a href="#"  class="icon"><i class="fa fa-facebook"></i></a>
            <a href="#" class="icon"><i class="fa fa-twitter"></i></a>
            <a href="#" class="icon"><i class="fa fa-instagram"></i></a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Home  from './components/Home.vue'

export default {
  name: 'app',
  components: {
    Nav,
    Home
  }
}
</script>

<style lang='sass'>
@import '../node_modules/bulma/bulma.sass'
@import './mediaquerys'

.footer
  background-color: $dark 
  color: #f3f3f3
  .icon
    color: $warning
    margin-left: 1rem
</style>
