<template>
     <!-- Women Banner Section Begin -->
    <section class="women-banner spad">
        <div class="container-fluid">
            <div class="row">
                <div class="col-lg-12 mt-5">
                    <carousel class="product-slider" :margin="25" :loop="true" :stagePadding="100" :autoplay="true" :nav="false">

                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/terkait-1.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active"> 
                                        <a href="#">+<i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view"><router-link to="/product">Lihat Detail</router-link></li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Desain</div>
                                <a href="#">
                                    <h5>Packaging Bento</h5>
                                </a>
                                <div class="product-price">
                                    Rp.15.000,-
                                </div>
                            </div>
                        </div>
                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/terkait-2.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active">
                                        <a href="#">+<i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view"><a href="#">Lihat Detail</a></li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Desain</div>
                                <a href="#">
                                    <h5>Packaging Mug/Gelas</h5>
                                </a>
                                <div class="product-price">
                                    Mulai dari Rp.30.000,-
                                </div>
                            </div>
                        </div>
                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/terkait-3.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active">
                                        <a href="#">+<i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view"><a href="#">Lihat Detail</a></li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Desain</div>
                                <a href="#">
                                    <h5>Packaging Onigiri</h5>
                                </a>
                                <div class="product-price">
                                    Rp.60.000,-
                                </div>
                            </div>
                        </div>
                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/terkait-4.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active">
                                        <a href="#">+<i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view"><a href="#">Lihat Detail</a></li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Desain</div>
                                <a href="#">
                                    <h5>Packaging Minuman</h5>
                                </a>
                                <div class="product-price">
                                    Rp.75.000,-
                                </div>
                            </div>
                        </div>

                    </carousel>
                </div>
            </div>
        </div>
    </section>
    <!-- Women Banner Section End -->
</template>

<script>

import carousel from 'vue-owl-carousel'

export default {
    name: 'RelatedKesra',
    components: {
    carousel
   }
}
</script>

<style scoped>

</style>