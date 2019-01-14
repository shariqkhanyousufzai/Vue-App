<template>
  <div id="app">
    <div class="navbar  ">
      <div class="container">
        <div class="navbar-start">
          <a class="navbar-item">J-Axis</a>
        </div>
        <span class="navbar-burger" v-on:click="burgerNav" v-bind:class="{'is-active': isActive}">
          <span></span>
          <span></span>
          <span></span>
        </span>
        <div class="navbar-end navbar-menu myhamsetting" v-bind:class="{'is-active': isActive}">
          <router-link to="/" class="navbar-item r-item">Home</router-link>
          <router-link to="faq" class="navbar-item r-item">Features</router-link>
          <router-link to="faq" class="navbar-item r-item">About</router-link>
          <router-link to="faq" class="navbar-item r-item">FAQ</router-link>
          <div class="navbar-item">
            <p class="control">
              <a class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fa fa-download" aria-hidden="true"></i>
                </span>
                <span>join now

                </span>
              </a>
            </p>
          </div>
        </div>
      </div>
    </div>
    <router-view/>
    <footer class="footer is primary">
      <div class="container">
        <div class="columns">
          <div class="column">
            <p>And this right here is a spiffy footer, where you can put stuff.</p>
          </div>
          <div class="column has-text-right">
            <a class="icon" href="#"><i class="fab fa-facebook" aria-hidden="true"></i></a>
            <a class="icon" href="#"><i class="fab fa-twitter"></i></a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data: function(){
    return{
      isActive: false
    }
  },
  methods:{
    burgerNav: function(){
      this.isActive = !this.isActive;
    }
  }
}

</script>

<style lang="sass">
@import '../node_modules/bulma/bulma.sass'
@import 'mq'

.navbar
 background-color: #383838 
 a:hover
   color:gray

.navbar-start
  display: inline-block
  float: left

.navbar-start a
  color:#fff
  font-weight: bold
  font-size: 24px
a.r-item
  color:#C1C1C1
  padding: 0.5rem 1.7rem
  +mobile
  color:gray
    &:hover
      background-color:#F1F1F1
.myhamsetting    
    z-index: 1
    position: absolute
    width: 100%
  
.navbar-burger span
  background-color:#C1C1C1

footer
  background-color: $primary !important
  color: #fff
  .icon
   color: #fff
   margin-left: 20px 
   padding: 4% 0%


</style>
