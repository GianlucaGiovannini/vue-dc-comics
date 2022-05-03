<template>
    <div class="merc_banner">
        <div class="container">
            <div class="row row-cols-1 row-cols-md-3 row-cols-lg-5 py-4">
                <div class="col" v-for="({src, text}, index) in mercandise" :key="index">
                    <a href="#">
                        <img :src="src" :alt="'merce' + text">
                        <span>{{ text }}</span>
                    </a>
                </div>
                <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
                
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
                    src: "@/assets/img/buy-comics-digital-comics.png",
                    text: "digital comics"
                },
                {
                    src: "@/assets/img/buy-comics-merchandise.png",
                    text: "Dc Merchandise"
                },
                {
                    src: "@/assets/img/buy-comics-subscriptions.png",
                    text: "subscription"
                },
                {
                    src: "@/assets/img/buy-comics-shop-locator.png",
                    text: "comic shop locator"
                },
                {
                    src: "@/assets/img/buy-dc-power-visa.svg",
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
     

    a {
        color: $bannerTextColor; 
        text-decoration: none;
    }
}
</style>