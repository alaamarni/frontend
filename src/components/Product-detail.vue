<template>
  <div> 
    <div class="row">
      <div class="col-lg-12">
        <div class="card">
          <div class="card-body">
            <div class="row">
              <div class="col-xl-5">
                <div class="product-detail">
                  <div class="row">
                    <div class="col-3">
                      <div
                        class="nav flex-column nav-pills"
                        id="v-pills-tab"
                        role="tablist"
                        aria-orientation="vertical"
                      >
                        <a
                          class="nav-link"
                          id="product-1-tab"
                          data-toggle="pill"
                          @click="imageShow($event)"
                          role="tab"
                        >
                          <img
                            src="@/assets/images/product/img-1.png"
                            alt
                            class="img-fluid mx-auto d-block tab-img rounded"
                          />
                        </a>
                        <a
                          class="nav-link"
                          id="product-2-tab"
                          data-toggle="pill"
                          @click="imageShow($event)"
                          role="tab"
                        >
                          <img
                            src="@/assets/images/product/img-5.png"
                            alt
                            class="img-fluid mx-auto d-block tab-img rounded"
                          />
                        </a>
                        <a
                          class="nav-link"
                          id="product-3-tab"
                          data-toggle="pill"
                          @click="imageShow($event)"
                          role="tab"
                        >
                          <img
                            src="@/assets/images/product/img-3.png"
                            alt
                            class="img-fluid mx-auto d-block tab-img rounded"
                          />
                        </a>
                        <a
                          class="nav-link"
                          id="product-4-tab"
                          data-toggle="pill"
                          @click="imageShow($event)"
                          role="tab"
                        >
                          <img
                            src="@/assets/images/product/img-4.png"
                            alt
                            class="img-fluid mx-auto d-block tab-img rounded"
                          />
                        </a>
                      </div>
                    </div>
                    <div class="col-md-8 col-9">
                      <div class="tab-content" id="v-pills-tabContent">
                        <div class="tab-pane fade show active" id="product-1" role="tabpanel">
                          <div class="product-img">
                            <img
                              id="expandedImg"
                              src="@/assets/images/product/img-1.png"
                              alt
                              class="img-fluid mx-auto d-block"
                            />
                          </div>
                        </div>
                      </div>
                      <div class="row text-center mt-2">
                        <div class="col-sm-6">
                          <button
                            type="button"
                            class="btn btn-primary btn-block waves-effect waves-light mt-2 mr-1"
                          >
                            <i class="mdi mdi-cart mr-2"></i> Add to cart
                          </button>
                        </div>
                        <div class="col-sm-6">
                          <button
                            type="button"
                            class="btn btn-light btn-block waves-effect mt-2 waves-light"
                          >
                            <i class="mdi mdi-shopping mr-2"></i>Buy now
                          </button>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <!-- end product img -->
              </div>
              <div class="col-xl-7">
                <div class="mt-4 mt-xl-3">
                  <a href="#" class="text-primary">T-shirt</a>
                  <h5 class="mt-1 mb-3">Full sleeve Blue color t-shirt</h5>

                  <div class="d-inline-flex">
                    <div class="text-muted mr-3">
                      <span class="mdi mdi-star text-warning"></span>
                      <span class="mdi mdi-star text-warning"></span>
                      <span class="mdi mdi-star text-warning"></span>
                      <span class="mdi mdi-star text-warning"></span>
                      <span class="mdi mdi-star"></span>
                    </div>
                    <div class="text-muted">( 132 )</div>
                  </div>

                  <h5 class="mt-2">
                    <del class="text-muted mr-2">$252</del>$240
                    <span class="text-danger font-size-12 ml-2">25 % Off</span>
                  </h5>
                  <p
                    class="mt-3"
                  >To achieve this, it would be necessary to have uniform pronunciation</p>
                  <hr class="my-4" />

                  <div class="row">
                    <div class="col-md-6">
                      <div>
                        
                      

                        <h5 class="font-size-14">Description :</h5>
                        <ul class="list-unstyled product-desc-list">
                          <li>
                            <i class="mdi mdi-circle-medium mr-1 align-middle"></i> Full Sleeve
                          </li>
                          <li>
                            <i class="mdi mdi-circle-medium mr-1 align-middle"></i> Cotton
                          </li>
                          <li>
                            <i class="mdi mdi-circle-medium mr-1 align-middle"></i> All Sizes available
                          </li>
                          <li>
                            <i class="mdi mdi-circle-medium mr-1 align-middle"></i> 4 Different Color
                          </li>
                        </ul>
                      </div>
                    </div>

                    <div>
                      <h5 class="font-size-14">Services :</h5>
                      <ul class="list-unstyled product-desc-list">
                        <li>
                          <i class="mdi mdi-sync text-primary mr-1 align-middle font-size-16"></i> 10 Days Replacement
                        </li>
                        <li>
                          <i
                            class="mdi mdi-currency-usd-circle text-primary mr-1 align-middle font-size-16"
                          ></i> Cash on Delivery available
                        </li>
                      </ul>
                    </div>
                  </div>

            
                </div>
              </div>
            </div>
            <!-- end row -->

         

          </div>
        </div>
        <!-- end card -->
      </div>
    </div>
    <!-- end row -->

  </div>  
</template>