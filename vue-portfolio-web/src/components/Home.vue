<template>
<section class="hero is-success is-fullheight">
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
        {{heading}}
      </h1>
      <h2 class=" is-two-thirds column is-paddingless">
        <h3 class="subtitle is-4">
          {{subheading}}
        </h3>
      </h2>
      <a href="#" class="button is-warning is-outlined is-large">Get in touch now</a>
    </div>
  </div>
</section>
</template>

<script>
export default {
  name: 'Home',
  data(){
    return{
      heading: 'Ismael Garcia ',
      subheading: 'Im a jr.Web Developer and an ardent learner who is always creating and learning awesome stuff. Lets start scrolling and learn more about me.'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='sass' scoped >
@import '../mediaquerys'
.hero
  background: linear-gradient(to top, rgba($primary, 0.4) ,rgba(#000 , 0.8) ), url('../assets/farzad-nazifi-71686-unsplash.jpg') center no-repeat
  background-size: cover
  background-attachment: fixed
  .title
    text-transform: uppercase
    line-heigth: 150%
    letter-spacing: 2px
    font-family: 'Helvetica',Roboto
    +mobile
      font-weight: bold
    +tablet
      font-size: 2rem
    +desktop
      font-size: 4rem
.container .button
  margin-top: 2rem
  transition: background 0.3s ease-in-out

  

</style>
