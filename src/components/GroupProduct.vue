<template>
     <div class="col-lg-9">
        <div class="card">
          <div class="card-body">
            <div>
              <div class="row">
                <div class="col-md-6">
                  <div>
                    <h5>Nos Produits</h5>
                   
                  </div>
                </div>

                <div class="col-md-6">
                  <div class="form-inline float-md-right">
                    <div class="search-box ml-2">
                      <div class="position-relative">
                        <input type="text" class="form-control rounded" placeholder="Search..." />
                        <i class="mdi mdi-magnify search-icon"></i>
                      </div>
                    </div>
                  </div>
                </div>
              </div>

              
              <div class="row no-gutters" style>
                <div class="col-xl-4 col-sm-6" v-for="(category,idx) in categories" 
                     :key="category.id" :class="{ active: idx==0 }">
                  <div class="product-box"  >
                    <div class="product-img">
                      <div class="product-ribbon badge badge-warning"></div>
                     
                      <img
                        :src="category.img"
                        alt
                        class="img-fluid mx-auto d-block"
                      />
                    </div>

                    <div class="text-center">
                      <p class="font-size-12 mb-1">{{category.name}}</p>
                      

                      <h5 class="mt-3 mb-0">{{category.price}}€</h5>
                    
                    </div>
                    <br>
                     <button type="button" class="btn btn-primary  btn-block" style="padding:1% 5%;"><i class="mdi mdi-cart mr-2"></i> Ajouter au Panier</button>

                  </div>
                </div>

               
                

              
              </div>

              
            </div>
          </div>
        </div>
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
      const res = await axios.get(`http://127.0.0.1:8000/api/product`);

      this.categories = res.data;
    } catch (e) {
      console.error(e);
    }
  },
  }
</script>