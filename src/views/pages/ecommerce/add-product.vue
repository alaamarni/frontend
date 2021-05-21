<script>
import AddProduct from "../../../components/AddProduct";
import Header from "../../../components/Header";
import Footer from "../../../components/footer";

/**
 * Product Detail Component
 */
export default {
  components: {
    Header,
    AddProduct,
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
        <AddProduct />
        <Footer />
  </div>
   
  
</template>