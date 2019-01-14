<template>
  <div class="home">
    <section class="hero is-primary">
  <div class="hero-body">
    <div class="container">
      <h1 class="title">
        FAQ
      </h1>
      <h2 class="subtitle">
        Lorem Ipsum is simply dummy text of the printing and typesetting industry
      </h2>
   
    </div>
  
  </div>
  </section>
  
    <section>
      <div class="container mysection-3">
       <div class="columns" v-if="faqs && faqs.length">
          <div class="column is-one-third" v-bind:key="faq" v-for="faq of faqs">
            <div class="card">
              <div class="card-content">
                <p class="title">{{ faq.title }}</p>
                <p class="answer">{{ faq.body }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>    

    </section>
    
  </div>
</template>

<script>
import axios from 'axios';
export default {
  name: 'faq',
  data:()=>({
    faqs:[],
    errors:[]
  }),
  created(){
    axios.get('http://jsonplaceholder.typicode.com/posts')
    .then(response =>{
      this.faqs = response.data.slice(0,20);
    })
    .catch(e=>{
      this.errors.push(e)
    })
  }
  
}
</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.hero-body
  background-color:#fff!important

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
.columns  
  flex-wrap: wrap

  
</style>