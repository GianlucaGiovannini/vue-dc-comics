<template>
    <div class="merc_banner">
        <div class="container">
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-xl-5 py-5">
                <div class="col my-3" v-for="item in merchandise" :key="item.id">
                    <a href="#" class="d-flex align-items-center">
                        <img :src="item.src" :alt="'merce ' + item.text">
                        <span class="ms-2 text-uppercase">{{ item.text }}</span>
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
            merchandise: [
                {
                    id: 1,
                    src: require("@/assets/img/buy-comics-digital-comics.png"),
                    text: "digital comics"
                },
                {
                    id: 2,
                    src: require("@/assets/img/buy-comics-merchandise.png"),
                    text: "Dc Merchandise"
                },
                {
                    id: 3,
                    src: require("@/assets/img/buy-comics-subscriptions.png"),
                    text: "subscription"
                },
                {
                    id: 4,
                    src: require("@/assets/img/buy-comics-shop-locator.png"),
                    text: "comic shop locator"
                },
                {
                    id: 5,
                    src: require("@/assets/img/buy-dc-power-visa.svg"),
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
    z-index: 1;
    img {
            width: auto;
            max-height: 55px;
            z-index: 1;
        }

    a {
        color: $bannerTextColor; 
        text-decoration: none;
        z-index: 1;

       span {
           font-size: 0.8rem;
           z-index: 1;
       }
    }
}
</style>