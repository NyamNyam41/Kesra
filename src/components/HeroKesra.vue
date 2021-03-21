<template>
    <!-- Hero Section Begin -->
    <section class="hero-section">
        <carousel class="hero-items" :loop="true" :items="1" :autoplay="true" :nav="false" :dots="false" :autoplaySpeed="3" :autoplayHoverPause="true">

            <div class="single-hero-items set-bg" style="background-image: url('/img/hero-1.jpg')">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-5">
                            <span>Packaging, UI, Banner, Flyer </span>
                            <h1>Desain</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore
                            </p>
                            <button v-on:click="$emit('item-scroll')" class="primary-btn">Pesan Sekarang</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="single-hero-items set-bg" style="background-image: url('/img/hero-2.jpg')">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-5">
                            <span>Foto dan video produk, acara, dll </span>
                            <h1>Foto & Video</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore
                            </p>
                            <button v-on:click="$emit('item-scroll')" class="primary-btn">Pesan Sekarang</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="single-hero-items set-bg" style="background-image: url('/img/hero-3.jpg')">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-5">
                            <span>Komputer, Smartphone, Instalasi</span>
                            <h1>Reparasi</h1>
                            <p>
                                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore
                            </p>
                           <button v-on:click="$emit('item-scroll')" class="primary-btn">Pesan Sekarang</button>
                        </div>
                    </div>
                </div>
            </div>
            
        </carousel>
    </section>
    <!-- Hero Section End -->
</template>

<script>

import carousel from 'vue-owl-carousel'

export default {

   name: 'HeroKesra',
   components: {
    carousel
   }
    
}
</script>

<style scoped>

.primary-btn{
    border: 0px;
}

</style>