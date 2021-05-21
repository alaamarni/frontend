<script>

import Header from "../../../components/Header";

import GroupProduct from "../../../components/GroupProduct";


import Footer from '../../../components/footer.vue';

/**
 * Products Component
 */
export default {
  page: {
    title: "Product",
   
  },
  components: {
    
    Header,
    Footer,
    
    GroupProduct
    
   
   
  },
 
 
};
</script>

<template>
<div>
  <Header />
  <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <div class="row">
      <div class="col-xl-3 col-lg-4">
        <div class="card">
          <div class="card-header bg-transparent border-bottom">
            <h5 class="mb-0">BeHerbe</h5>
          </div>

          <div class="card-body">
            <h5 class="font-size-14 mb-3">Categories</h5>

            <div id="accordion" class="custom-accordion categories-accordion mb-3">
              <div class="categories-group-card">
                <a v-b-toggle.electorinic class="categories-group-list">
                  Produit de la Ruche
                  <i class="mdi mdi-minus float-right accor-plus-icon"></i>
                </a>

                <b-collapse id="electorinic" data-parent="#accordion" accordion="my-accordion">
                  <div>
                    <ul class="list-unstyled categories-list mb-0">
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Miel Bio
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Miel Conventionelle
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Manuka
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Propolis
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Pollen
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Gélée Royale
                        </a>
                      </li>
                    </ul>
                  </div>
                </b-collapse>
              </div>

              <div class="categories-group-card">
                <a
                  v-b-toggle.fashion
                  class="categories-group-list"
                  data-toggle="collapse"
                  aria-expanded="true"
                  aria-controls="collapseTwo"
                >
                  Plante Medicinal
                  <i class="mdi mdi-minus float-right accor-plus-icon"></i>
                </a>
                <b-collapse id="fashion" visible data-parent="#accordion" accordion="my-accordion">
                  <div>
                    <ul class="list-unstyled categories-list mb-0">
                      <li class="active">
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Vrac Capsule
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Extrait
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Gellules
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Tablet
                        </a>
                      </li>
                    </ul>
                  </div>
                </b-collapse>
              </div>

              <div class="categories-group-card">
                <a
                  v-b-toggle.kids
                  class="categories-group-list collapsed"
                  data-toggle="collapse"
                  aria-expanded="false"
                  aria-controls="collapseThree"
                >
                  Aromatherapie
                  <i class="mdi mdi-minus float-right accor-plus-icon"></i>
                </a>
                <b-collapse id="kids" data-parent="#accordion" accordion="my-accordion">
                  <div>
                    <ul class="list-unstyled categories-list mb-0">
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Huile Vegetale
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Huile Essentielle
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Hydrolate
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i>Diffuseur du Parfum
                        </a>
                      </li>
                    </ul>
                  </div>
                </b-collapse>
              </div>

              <div class="categories-group-card">
                <a
                  v-b-toggle.Fitness
                  class="categories-group-list collapsed"
                  data-toggle="collapse"
                  aria-expanded="false"
                  aria-controls="collapseFour"
                >
                  Cosmetique Bio
                  <i class="mdi mdi-minus float-right accor-plus-icon"></i>
                </a>
                <b-collapse id="Fitness" data-parent="#accordion" accordion="my-accordion">
                  <div>
                    <ul class="list-unstyled categories-list mb-0">
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Soins cheveux
                        </a>
                      </li>
                         <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Soins du corps
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Soins de la peau
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Soins des mains
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Soins du visage
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Maquillage
                        </a>
                      </li>
                   
                     
                     
                    </ul>
                  </div>
                </b-collapse>
              </div>


              <div class="categories-group-card">
                <a
                  v-b-toggle.Fitness
                  class="categories-group-list collapsed"
                  data-toggle="collapse"
                  aria-expanded="false"
                  aria-controls="collapseFour"
                >
                   Compliment Alimentaire
                  <i class="mdi mdi-minus float-right accor-plus-icon"></i>
                </a>
                <b-collapse id="Fitness" data-parent="#accordion" accordion="my-accordion">
                  <div>
                    <ul class="list-unstyled categories-list mb-0">
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Vitamine
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Sels Minéraux
                        </a>
                      </li>
                     
                     
                    </ul>
                  </div>
                </b-collapse>
              </div>


              <div class="categories-group-card">
                <a
                  v-b-toggle.Fitness
                  class="categories-group-list collapsed"
                  data-toggle="collapse"
                  aria-expanded="false"
                  aria-controls="collapseFour"
                >
                  Gemmotherapie
                  <i class="mdi mdi-minus float-right accor-plus-icon"></i>
                </a>
                <b-collapse id="Fitness" data-parent="#accordion" accordion="my-accordion">
                  <div>
                    <ul class="list-unstyled categories-list mb-0">
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Sérum
                        </a>
                      </li>
                      <li>
                        <a href="#">
                          <i class="mdi mdi-circle-medium mr-1"></i> Gouttes
                        </a>
                      </li>
                     
                     
                    </ul>
                  </div>
                </b-collapse>
              </div>
            </div>
          </div>

          

          <div class="custom-accordion">
            



          </div>
        </div>
      </div>

<GroupProduct />

      
     
    </div>
     <div class="container">
  
</div>
    <Footer />
    <!-- end row -->
  </div>
</template>