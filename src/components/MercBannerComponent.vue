<template>
    <div class="merc_banner">
        <div class="container">
            <div class="row row-cols-1 row-cols-md-3 row-cols-xl-5 py-5">
                <div class="col my-3" v-for="({src, text}, index) in mercandise" :key="index">
                    <a href="#" class="d-flex align-items-center">
                        <img :src="require(`@/assets${src}`)" :alt="'merce' + text">
                        <span class="ms-2 text-uppercase">{{ text }}</span>
                    </a>
                </div>
                <!-- <div class="col my-3 p-0">
                    <a href="#" class="d-flex align-items-center">
                        <img src="@/assets/img/buy-comics-digital-comics.png">
                        <span class="ms-2 text-uppercase">digital comics</span>
                    </a>
                </div>
                <div class="col my-3 p-0">
                    <a href="#" class="d-flex align-items-center">
                        <img src="@/assets/img/buy-comics-merchandise.png">
                        <span class="ms-2 text-uppercase">Dc Merchandise</span>
                    </a>
                </div>
                <div class="col my-3 p-0">
                    <a href="#" class="d-flex align-items-center">
                        <img src="@/assets/img/buy-comics-subscriptions.png">
                        <span class="ms-2 text-uppercase">subscription</span>
                    </a>
                </div>
                <div class="col my-3 p-0">
                    <a href="#" class="d-flex align-items-center">
                        <img src="@/assets/img/buy-comics-shop-locator.png">
                        <span class="ms-2 text-uppercase">comic shop locator</span>
                    </a>
                </div>
                <div class="col my-3 p-0">
                    <a href="#" class="d-flex align-items-center">
                        <img src="@/assets/img/buy-dc-power-visa.svg">
                        <span class="ms-2 text-uppercase">dc power visa</span>
                    </a>
                </div> -->

                
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MercBannerComponent',
    data() {
        return {
            mercandise: [
                {
                    src: "/img/buy-comics-digital-comics.png",
                    text: "digital comics"
                },
                {
                    src: "/img/buy-comics-merchandise.png",
                    text: "Dc Merchandise"
                },
                {
                    src: "/img/buy-comics-subscriptions.png",
                    text: "subscription"
                },
                {
                    src: "/img/buy-comics-shop-locator.png",
                    text: "comic shop locator"
                },
                {
                    src: "/img/buy-dc-power-visa.svg",
                    text: "dc power visa"
                },
            ],
        };   
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/variables';
.merc_banner {
    background-color: $primaryColor;  
    
    img {
            width: auto;
            max-height: 55px;
        }

    a {
        color: $bannerTextColor; 
        text-decoration: none;

       span {
           font-size: 0.8rem;
       }
    }
}
</style>