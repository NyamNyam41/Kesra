<template>
    
 <!-- Footer Section Begin -->
    <footer class="footer-section">
        <div class="container">
            <div class="row">
                
                    <div class="col-lg-5 footer-left text-left">
                        <div class="footer-logo">
                            <a href="#"><img src="img/logo_website_shayna_white.png" alt="" /></a>
                        </div>
                        <ul>
                            <li>Alamat: Yogyakarta, Indonesia</li>
                            <li>Telepon: +628 22081996</li>
                            <li>Email: hello.kreska@gmail.com</li>
                        </ul>
                        <div class="footer-social ">
                            <a href="#"><i class="fa fa-facebook"></i></a>
                            <a href="#"><i class="fa fa-instagram"></i></a>
                            <a href="#"><i class="fa fa-twitter"></i></a>
                            <a href="#"><i class="fa fa-pinterest"></i></a>
                        </div>
                    </div>
               
                <div class="col-lg-3 offset-lg-1 text-left">
                    <div class="footer-widget">
                        <h5>Informasi</h5>
                        <ul>
                            <li><a href="#">Tentang Kami</a></li>
                            <li><a href="#">Kontak</a></li>
                            <li><a href="#">Keluhan</a></li>
                            <li><a href="#">Lainnya</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-3 text-left">
                    <div class="footer-widget">
                        <h5>Sponsor</h5>
                        <ul>
                            <li><a href="#">Mangrove</a></li>
                            <li><a href="#">Kupiku</a></li>
                            <li><a href="#">Jogpair</a></li>
                            <li><a href="#">Ortindo</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="copyright-reserved">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12">
                        <div class="copyright-text">
                            Hak Cipta &copy;
                            {{currentYear}} | Kreska - Kreasi Kewirausahaan SMK
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
 <!-- Footer Section End -->

</template>

<script>



export default {
    name :'FooterKesra',
    data() {
        return {
        currentYear: new Date().getFullYear(),
        }
    }
}
</script>

<style scoped>

</style>