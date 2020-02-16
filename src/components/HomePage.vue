<template>
  <div>
     <img  src="./reddit.jpg"/>
    <h1>"Welcome to Your Vue.js APP Tosh " </h1>
      <div>
        <h2>Home Page</h2>
        <div class="container">
            <div class="row">
                <div v-for="image in latest" v-bind:key="image" class="col-lg-3">
                  <ImageCard/>
             </div>
        </div>
    </div>
  </div>
  </div>
</template>

<script>
import ImageCard from './ImageCard'
export default {
  name: 'HomePage',
  components:{
    ImageCard
  },
   data() {
        return {
            latest: [
            "./airplane.jpg",
            "./airplane.jpg",
            "./airplane.jpg",
            "./airplane.jpg",
            "./airplane.jpg",
            "./airplane.jpg",
            ]
        }
  }
}
</script>

<style>
</style>
