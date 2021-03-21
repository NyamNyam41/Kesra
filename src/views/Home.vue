<template>
  <div class="home">
      <HeaderKesra />
      
      <HeroKesra @item-scroll="itemScroll('pep1')"/>
      
       <!-- separator start -->
        <div class="container">
          <div class="row">
            <div class="col mt-5 mb-1">
              <h2 class="text-divider"><span>Jasa dan Produk Kreasi Kewirausahaan SMK</span></h2>
            </div>
          </div>
        </div>
      <!-- separator end -->

      <div ref="pep1">
      <ItemKesra/>
      </div>

     <FooterKesra />
  </div>
</template>

<script>


// @ is an alias to /src

import HeaderKesra from '@/components/HeaderKesra.vue'
import HeroKesra from '@/components/HeroKesra.vue'
import ItemKesra from '@/components/ItemKesra.vue'
import FooterKesra from '@/components/FooterKesra.vue'

export default {
  name: 'Home',
  components: {
    HeaderKesra,
    HeroKesra,
    ItemKesra,
    FooterKesra
  },
  methods:{
    itemScroll(refName){
      var element = this.$refs[refName];
      var top = element.offsetTop;
        window.scrollTo(0, top);
    }
  }
}
</script>
