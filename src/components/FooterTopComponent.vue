<template>
            <div class="footer_top py-5 position-relative">
            <div class="container">
                <div class="row row-cols-1 row-cols-sm-2">
                    <div class="col footer_list">
                        <div class="row row-cols-3">
                            <div class="col">
                                <div class="dc_comics_list">
                                    <h4 class="text-white py-2">DC Comics</h4>
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
                                </div>
                                <div class="shop_list">
                                    <h4 class="text-white py-2">SHOP</h4>
                                    <ul>
                                        <li>
                                            <a href="#">Shop DC</a>
                                        </li>
                                        <li>
                                            <a href="#">Shop DC Collectibles</a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="col">
                                <div class="dc_list">
                                    <h4 class="text-white py-2">DC</h4>
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
                            </div>
                            <div class="col">
                                <div class="sites_list">
                                    <h4 class="text-white py-2">SITES</h4>
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
            </div>
            <img class="img_footer_logo" src="@/assets/img/dc-logo-bg.png">
        </div>
</template>

<script>
export default {
    name: "FooterTopComponent",

    data() {
        return {
            dcComicsList: ["Characters","Comics", "Movie", "TV", "Games", "Videos", "News"],
            shopList: ["Shop DC","Shop DC Collectibles"],
            dcList: ["Terms of Use","Privacy policy (New)", "Ad Choise", "Advertising", "Jobs", "Subscription", "Talent Workshops", "CPSC Certificates", "Rating", "Shop Help", "Contact Us"],
            sitesList: ["DC","MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
        };
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/variables';

.footer_top {
        background-image: url("@/assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        

        .img_footer_logo{
            position: absolute;
            top: 50%;
            right: 0;
            transform: translate(0, -50%);
            z-index: 0;
        }

        .footer_list {
            z-index: 1;
            ul {
            list-style: none;
            padding:0;

                li {
                    padding: 0.2rem 0;
                    
                    a {
                        color: $footerTextLi;
                        text-decoration: none;
                        z-index: 1;

                        &:hover {
                            color: $primaryColor;
                        }
                    }
                }
            }
        }
    }  
</style>