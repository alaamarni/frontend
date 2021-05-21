<script>

import Header from "../../components/Header";
import Carrousel from '../../components/carrousel.vue';
import Nvproduct from '../../components/nvproduct.vue';
import Video from '../../components/video.vue';
import BrandCarrousel from '../../components/BrandCarrousel.vue';
import Footer from '../../components/footer.vue';

/**
 * Dashboard component
 */
export default {
  components: {
   
    Header,
    Carrousel,
    Nvproduct,
    Video,
    BrandCarrousel,
    Footer
    
   
  },
  data() {
    return {
      title: "Dashboard",
      items: [
        {
          text: "Nazox"
        },
        {
          text: "Dashboard",
          active: true
        }
      ]
    };
  }
};
</script>

<template>
<div>
  <Header />
  <Carrousel />  
  <Nvproduct />
  <Video />
  <BrandCarrousel />
  <br>
  <br>
  <br>
  <br>
  <br>
  <Footer />
  
</div>  
  </template>