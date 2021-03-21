<template>
  <div class="product">
      <HeaderKesra />

        <!-- Breadcrumb Section Begin -->
        <div class="breacrumb-section">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12">
                        <div class="breadcrumb-text product-more text-left">
                            <router-link to="/"><i class="fa fa-home"></i> Home</router-link>
                            <span>Detail</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Breadcrumb Section Begin -->

        <!-- Product Shop Section Begin -->
        <section class="product-shop spad page-details">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12">
                        <div class="row">
                            <div class="col-lg-6">
                                <div class="product-pic-zoom">
                                    <img class="product-big-img" :src="foto_default" alt="" />
                                </div>
                                <div class="product-thumbs">
                                    <carousel class="product-thumbs-track ps-slider" :dots="false" :margin="10" :stagePadding="13" :autoplay="true" :nav="false">
                                        <div class="pt" @click="changeFoto(thumbs[0])" :class="thumbs[0]==foto_default ? 'active' : '' ">
                                            <img src="img/mickey1.jpg" alt="" />
                                        </div>

                                        <div class="pt" @click="changeFoto(thumbs[1])" :class="thumbs[1]==foto_default ? 'active' : '' ">
                                            <img src="img/mickey2.jpg" alt="" />
                                        </div>

                                        <div class="pt" @click="changeFoto(thumbs[2])" :class="thumbs[2]==foto_default ? 'active' : '' ">
                                            <img src="img/mickey3.jpg" alt="" />
                                        </div>

                                        <div class="pt" @click="changeFoto(thumbs[3])" :class="thumbs[3]==foto_default ? 'active' : '' ">
                                            <img src="img/mickey4.jpg" alt="" />
                                        </div>
                                    </carousel>
                                </div>
                            </div>
                            <div class="col-lg-6">
                                <div class="product-details">
                                    <div class="pd-title text-left">
                                        <span>Desain</span>
                                        <h3>Packaging Makanan Ringan</h3>
                                    </div>
                                    <div class="pd-desc text-left">
                                        <p>
                                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, error
                                            officia. Rem aperiam laborum voluptatum vel, pariatur modi hic provident eum
                                            iure natus quos non a sequi, id accusantium! Autem.
                                        </p>
                                        <p>
                                            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quam possimus quisquam
                                            animi, commodi, nihil voluptate nostrum neque architecto illo officiis
                                            doloremque et corrupti cupiditate voluptatibus error illum. Commodi expedita
                                            animi nulla aspernatur.
                                            Id asperiores blanditiis, omnis repudiandae iste inventore cum, quam sint
                                            molestiae accusamus voluptates ex tempora illum sit perspiciatis. Nostrum dolor
                                            tenetur amet, illo natus magni veniam quia sit nihil dolores.
                                            Commodi ratione distinctio harum voluptatum velit facilis voluptas animi non
                                            laudantium, id dolorem atque perferendis enim ducimus? A exercitationem
                                            recusandae aliquam quod. Itaque inventore obcaecati, unde quam
                                            impedit praesentium veritatis quis beatae ea atque perferendis voluptates velit
                                            architecto?
                                        </p>
                                        <h4>Rp.15.000,-</h4>
                                    </div>
                                    <div class="quantity">
                                        <router-link to="/checkout" href="shopping-cart.html" class="primary-btn pd-cart">Masukkan Keranjang Belanja</router-link>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <!-- Product Shop Section End -->

        <!-- separator start -->
        <div class="container">
          <div class="row">
            <div class="col mt-5 mb-1">
              <h2 class="text-divider"><span>Produk Terkait</span></h2>
            </div>
          </div>
        </div>
        <!-- separator end -->

        <RelatedKesra />

     <FooterKesra />
  </div>
</template>

<script>

// @ is an alias to /src
import carousel from 'vue-owl-carousel'

import HeaderKesra from '@/components/HeaderKesra.vue'
import FooterKesra from '@/components/FooterKesra.vue'
import RelatedKesra from '@/components/RelatedKesra.vue'

export default {
  name: 'Product',
  components: {
    carousel,
    HeaderKesra,
    FooterKesra,
    RelatedKesra
  },
  data(){
      return {
          foto_default: "img/mickey1.jpg",
          thumbs: [
              "img/mickey1.jpg",
              "img/mickey2.jpg",
              "img/mickey3.jpg",
              "img/mickey4.jpg"
          ]
      }
  },
  methods : {
      changeFoto(url_image){
          this.foto_default = url_image;
      }
  }
}
</script>
