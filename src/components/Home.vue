<template>

  <div class="home">

    <section class="hero is-primary">
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
        Soaring to new heights
      </h1>
      <h2 class="subtitle">
        Lorem Ipsum is simply dummy text of the printing and typesetting industry
      </h2>
      <a class="button is-large is-primary">Primary</a>
    </div>
  
  </div>
  </section>
  <section>
    <div class="container mysection-2">
     <div class="tile is-parent colum is-12 ">
      <article class="tile is-child notification  colum is-1">
        <p class="title mycog"><i class="fas fa-cog"></i></p>
        <p class="subtitle"></p>
        <div class="content">
          <!-- Content -->
        </div>
        
      </article>
      
       <article class="tile is-child notification  colum is-5">
        
        <p class="subtitle">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.</p>
        <div class="content">
          <!-- Content -->
        </div>
        
      </article>
      <article class="tile is-child notification  colum is-1">
        
      </article>
      <article class="tile is-child notification  colum is-5">
        
        <p class="section-2">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.</p>
        <div class="content">
          <!-- Content -->
        </div>
        
      </article>
    </div>
    </div>
    </section>
    <section>
      <div class="container mysection-3">
        <div class="tile is-parent colum is-12 ">
          <article class="tile is-child notification  colum is-1 ">
        
      </article>
        <article class="tile is-child notification is-warning colum is-3 section-3-box">
          <div class="box-pad">
          <p class="subtitle">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's.</p>
          <p class="title">-Grey Panter</p>
          </div>
        </article> 
        <article class="tile is-child notification  colum is-1">
        
      </article> 
        <article class="tile is-child notification is-warning colum is-3 section-3-box">
          <div class="box-pad">
          <p class="subtitle">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's.</p>
          <p class="title">-Grey Panter</p>
          </div>
        </article>  

        <article class="tile is-child notification  colum is-1">
        
      </article>
        <article class="tile is-child notification is-warning colum is-3 section-3-box">
          <div class="box-pad">
          <p class="subtitle">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's.</p>
          <p class="title">-Grey Panter</p>
          </div>
        </article>  
        </div>
      </div>      

    </section>
    
  </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.hero-body
  background: url('../assets/clouds.jpg')
  background: cover
  background-size: 100%
  padding: 9.5% 0%;

h1.title 
  color: #383838 !important  

h2.subtitle 
  color: #383838 !important

p.section-2
  line-height: 2.4

.mysection-2
  padding: 3% 0%
  background-color: #fff!important

.tile
   background-color: #fff!important

p.mycog
  line-height: 3

.section-3-box
  border: 1px solid #383838

.box-pad
  padding: 15px 4px
.mysection-3
  padding: 0% 0% 4% 0%
  
</style>