<template>
 <div class="checkout">

  <HeaderKesra/>

  <!-- Breadcrumb Section Begin -->
     <div class="breacrumb-section">
         <div class="container">
             <div class="row">
                 <div class="col-lg-12">
                     <div class="breadcrumb-text product-more text-left">
                         <router-link to="/"><i class="fa fa-home"></i>Home</router-link>
                         <span>Checkout</span>
                     </div>
                 </div>
             </div>
         </div>
     </div>
  <!-- Breadcrumb Section Begin -->

  <!-- Shopping Cart Section Begin -->
    <section class="shopping-cart spad">
        <div class="container">
            <div class="row">
                <div class="col-lg-8">
                    <div class="row">
                        <div class="col-lg-12">
                            <div class="cart-table">
                                <table>
                                    <thead>
                                        <tr>
                                            <th>Gambar</th>
                                            <th class="p-name text-center">Nama Produk</th>
                                            <th>Harga</th>
                                            <th>Aksi</th>
                                        </tr>
                                    </thead>
                                    <tbody>
                                        <tr>
                                            <td class="cart-pic first-row">
                                                <img src="img/cart-page/product-1.jpg" />
                                            </td>
                                            <td class="cart-title first-row text-center">
                                                <h5>Packaging Makanan Ringan</h5>
                                            </td>
                                            <td class="p-price first-row">Rp.15.000,-</td>
                                            <td class="delete-item"><a href="#"><i class="material-icons">
                                                        close
                                                    </i></a></td>
                                        </tr>
                                        <tr>
                                            <td class="cart-pic first-row">
                                                <img src="img/cart-page/product-2.jpg" />
                                            </td>
                                            <td class="cart-title first-row text-center">
                                                <h5>Desain Dashboard Admin Website</h5>
                                            </td>
                                            <td class="p-price first-row">Rp.60.000,-</td>
                                            <td class="delete-item"><a href="#"><i class="material-icons">
                                                        close
                                                    </i></a></td>
                                        </tr>
                                    </tbody>
                                </table>
                            </div>
                        </div>
                        <div class="col-lg-8 text-left">
                            <h4 class="mb-4">
                                Informasi Pembeli:
                            </h4>
                            <div class="user-checkout">
                                <form>
                                    <div class="form-group">
                                        <label for="namaLengkap">Nama lengkap</label>
                                        <input type="text" class="form-control" id="namaLengkap"
                                            aria-describedby="namaHelp" placeholder="Masukan Nama">
                                    </div>
                                    <div class="form-group">
                                        <label for="namaLengkap">Alamat email</label>
                                        <input type="email" class="form-control" id="emailAddress"
                                            aria-describedby="emailHelp" placeholder="Masukan Email">
                                    </div>
                                    <div class="form-group">
                                        <label for="namaLengkap">No. HP</label>
                                        <input type="text" class="form-control" id="noHP" aria-describedby="noHPHelp"
                                            placeholder="Masukan No. HP">
                                    </div>
                                    <div class="form-group">
                                        <label for="alamatLengkap">Alamat Lengkap</label>
                                        <textarea class="form-control" id="alamatLengkap" rows="3"></textarea>
                                    </div>
                                     <router-link to ="/sukses" class="primary-btn">Sudah Membayar</router-link>
                                </form>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4">
                    <div class="row">
                        <div class="col-lg-12">
                            <div class="proceed-checkout text-left">
                                <div class="proceed-btn">Detail Transaksi</div>
                                <ul>
                                    <li class="subtotal">ID Transaksi <span>#SH12000</span></li>
                                    <li class="subtotal mt-3">Total <span>Rp.75.000,-</span></li>
                                    <li class="subtotal mt-3">Pajak <span>10%</span></li>
                                    <li class="subtotal mt-3">Total Biaya <span>Rp.82.500,-</span></li>
                                    <li class="subtotal mt-3">Bank Transfer <span>Mandiri</span></li>
                                    <li class="subtotal mt-3">No. Rekening <span>2208 1996 1403</span></li>
                                    <li class="subtotal mt-3">Nama Penerima <span>Alia</span></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Shopping Cart Section End -->
    
 </div>
</template>

<script>

import HeaderKesra from '@/components/HeaderKesra.vue'

export default {
 name: 'Checkout',
 components:{
     HeaderKesra,
 }

}
</script>

<style scoped>

</style>