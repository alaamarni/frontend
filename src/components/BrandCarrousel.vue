<template>
  <div class="container">
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
     
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
       <div class="carousel-item" style="width:20%;" v-for="(category,idx) in categories" 
       :key="category.id" :class="{ active: idx==0 }">
          <img class="d-block img-fluid w-100" width="400" height="400"
           :src="category.img" alt="category.name">  
       </div>
    </b-carousel>
</div>
</template>

<script>
import axios from "axios";
  export default {
    data() {
      return {
         slide: 0,
        sliding: null,
         categories: []
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    },
     async created() {
    try {
      const res = await axios.get(`http://127.0.0.1:8000/api/category`);

      this.categories = res.data;
    } catch (e) {
      console.error(e);
    }
  },
  }
</script>