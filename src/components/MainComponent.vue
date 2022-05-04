<template>
    <main>
        <div class="container text-white">
            <div class="row row-cols-1">
                <div class="cols py-5 fs-4">
                    👉 Content goes here 👈
                </div>
            </div>
        </div>
        <MercBanner />
    </main>
</template>

<script>
import MercBanner from '@/components/MercBannerComponent.vue'
export default {
    name: 'MainComponent',
    components: {
        MercBanner
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/variables';
main {
    background-color: $mainBgColor;
    
}
</style>