<template>
    <div class="footer_bottom">
            <div class="container py-5">
                <div class="row row-cols-2 justify-content-around">
                    <div class="col">
                        <button class="btn_footer text-uppercase">Sign-up now!</button>
                    </div>
                    <div class="col d-flex gap-3 justify-content-end align-items-center">
                        <div class="text-uppercase follow_us">Follow us</div>
                        <a href="#">
                            <img src="@/assets/img/footer-facebook.png">
                        </a>
                        <a href="#">
                            <img src="@/assets/img/footer-twitter.png">
                        </a>                       
                        <a href="#">
                            <img src="@/assets/img/footer-youtube.png">
                        </a>                       
                        <a href="#">
                            <img src="@/assets/img/footer-pinterest.png">
                        </a>           
                        <a href="#">
                            <img src="@/assets/img/footer-periscope.png">
                        </a>     
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name: "FooterBottomComponent"
}
</script>

<style lang="scss" scoped>
.footer_bottom {
        background-color: $footerBanner;
        z-index: 1;

        .btn_footer{
            @include button;
            color: white;
            &:hover {
                box-shadow: inset 0 0 20px 0px $primaryColor;
            }
        }
        
        .follow_us {
            color: $primaryColor;
            font-weight: bold;
            margin-right: 1rem;
        }

        a {
            &:hover {
                transform: scale(1.3);
            }
        }
    }
</style>