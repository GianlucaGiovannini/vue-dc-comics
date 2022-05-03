<template>
    <div class="footer_bottom">
            <div class="container py-5">
                <div class="row row-cols-2 justify-content-around">
                    <div class="col">
                        <button class="btn_footer text-uppercase">Sign-up now!</button>
                    </div>
                    <div class="col d-flex gap-3 justify-content-end align-items-center">
                        <div class="text-uppercase follow_us">Follow us</div>
                        <img src="@/assets/img/footer-facebook.png">
                        <img src="@/assets/img/footer-twitter.png">
                        <img src="@/assets/img/footer-youtube.png">
                        <img src="@/assets/img/footer-pinterest.png">
                        <img src="@/assets/img/footer-periscope.png">
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
@import '@/assets/scss/variables';
.footer_bottom {
        background-color: $footerBanner;
        z-index: 1;

        .btn_footer{
            background-color: transparent;
            color: white;
            border: 2px solid $primaryColor;
            padding: 0.7rem;
            transition: 0.5s;

            &:hover {
                box-shadow: inset 0 0 20px 0px $primaryColor;
            }
        }
        
        .follow_us {
            color: $primaryColor;
            font-weight: bold;
            margin-right: 1rem;
        }
    }
</style>