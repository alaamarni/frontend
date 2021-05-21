<template>
    <div class="col-sm-12">
    <h2 class="my-5">Nouveaux Produits</h2>
        <div class="card-columns">
            <div v-for="category in categories" :key="category.id">
                <div class="card" style=" margin-left: auto;
                        margin-right: auto; ">
                    <img :src="category.img" alt="Image" class="d-flex justify-content-center align-items-center" style=" margin-left:auto;"  >
                        <div class="card-body">
                            <h4 class="card-title">
                                <h5 class="card-title">{{category.name}}</h5>
                            </h4>
                            <p class="card-text">{{category.description}}</p> 
                        </div>
                </div>    
            </div>   
        </div>
        <div class="d-flex justify-content-center align-items-center" >
                <button  type="button" class="btn btn-primary"> Plus de Produits <i class="zmdi zmdi-arrow-right"></i></button> 
        </div>
    </div>
</template>

<script>
import axios from "axios";


export default {

  data() {
    return {
      categories: []
    };
  },
   async created() {
    try {
      const res = await axios.get(`http://127.0.0.1:8000/api/nvproduct`);

      this.categories = res.data;
      this.responseAvailable = true;
    } catch (e) {
      console.error(e);
    }
  },
};
</script>