<template>
    <footer>
        <div class="footer_top py-5 position-relative">
            <div class="container">
                <div class="row row-cols-2">
                    <div class="col">
                        <div class="row row-cols-3">
                            <div class="col">
                                <h4 class="text-white py-3">DC Comics</h4>
                                <ul>
                                    <li>
                                        <a href="#">Characters</a>
                                    </li>
                                    <li>
                                        <a href="#">Comics</a>
                                    </li>
                                    <li>
                                        <a href="#">Movies</a>
                                    </li>
                                    <li>
                                        <a href="#">TV</a>
                                    </li>
                                    <li>
                                        <a href="#">Games</a>
                                    </li>
                                    <li>
                                        <a href="#">Videos</a>
                                    </li>
                                    <li>
                                        <a href="#">Characters</a>
                                    </li>
                                </ul>
                                <h4 class="text-white py-3">SHOP</h4>
                                <ul>
                                    <li>
                                        <a href="#">Shop DC</a>
                                        <a href="#">Shop DC Collectibles</a>
                                    </li>
                                </ul>
                            </div>
                            <div class="col">
                                <h4 class="text-white py-3">DC</h4>
                                <ul>
                                    <li>
                                        <a href="#">Terms Of Use</a>
                                    </li>
                                    <li>
                                        <a href="#">Privacy policy (New)</a>
                                    </li>
                                    <li>
                                        <a href="#">Ad Choices</a>
                                    </li>
                                    <li>
                                        <a href="#">Advertising</a>
                                    </li>
                                    <li>
                                        <a href="#">Jobs</a>
                                    </li>
                                    <li>
                                        <a href="#">Subscription</a>
                                    </li>
                                    <li>
                                        <a href="#">Talent Workshops</a>
                                    </li>
                                    <li>
                                        <a href="#">CPSC Certificates</a>
                                    </li>
                                    <li>
                                        <a href="#">Ratings</a>
                                    </li>
                                    <li>
                                        <a href="#">Shop Help</a>
                                    </li>
                                    <li>
                                        <a href="#">Contact Us</a>
                                    </li>
                                </ul>
                            </div>
                            <div class="col">
                                <h4 class="text-white py-3">SITES</h4>
                                <ul>
                                    <li>
                                        <a href="#">DC</a>
                                    </li>
                                    <li>
                                        <a href="#">MAD Magazine</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Kids</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Universe</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Power Visa</a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>                  
                </div>
            </div>
            <img class="img_footer_logo" src="@/assets/img/dc-logo-bg.png">
        </div>
        
        <div class="footer_bottom">
            <div class="container py-5">
                <div class="row row-cols-2 justify-content-around">
                    <div class="col">
                        <button class="text-uppercase">Sign-up now!</button>
                    </div>
                    <div class="col d-flex gap-3 justify-content-end align-items-center">
                        <div class="text-uppercase">Follow us</div>
                        <img src="@/assets/img/footer-facebook.png">
                        <img src="@/assets/img/footer-twitter.png">
                        <img src="@/assets/img/footer-youtube.png">
                        <img src="@/assets/img/footer-pinterest.png">
                        <img src="@/assets/img/footer-periscope.png">
                    </div>
                </div>

            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'FooterComponent',
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/variables';

footer {
    .footer_top {
        background-image: url("@/assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        z-index: -1;

        .img_footer_logo{
            position: absolute;
            top: 50%;
            right: 0;
            transform: translate(0, -50%);
            z-index: 0;
        }

        ul {
            list-style: none;
            padding:0;
        }
    }

    a {
        color: $footerTextLi;
        text-decoration: none;
    }

    .footer_bottom {
        background-color: $footerBanner;
        z-index: 1;

        .container{
            z-index: 1;
        }
        .row {
            z-index: 1;
        }
    }
}

</style>