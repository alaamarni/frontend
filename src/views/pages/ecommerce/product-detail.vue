<script>
import ProductDetail from "../../../components/Product-detail";
import Header from "../../../components/Header";
import Footer from "../../../components/footer";

/**
 * Product Detail Component
 */
export default {
  components: {
    Header,
    ProductDetail,
    Footer

  },
  data() {
    return {
      title: "Product Detail",
      items: [
        {
          text: "Ecommerce"
        },
        {
          text: "Product Detail",
          active: true
        }
      ]
    };
  },
  methods: {
    /**
     * Selected image shows
     */
    imageShow(event) {
      const image = event.target.src;
      const expandImg = document.getElementById("expandedImg");
      expandImg.src = image;
    }
  }
};
</script>

<template>
  
  <div>
        <Header />
        <ProductDetail />
        <Footer />
  </div>
   
  
</template>