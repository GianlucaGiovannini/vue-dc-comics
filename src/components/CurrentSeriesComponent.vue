<template>
    <div class="col">
        <div class="series_img">
            <img :src="thumb">
        </div>
        <div class="category text-uppercase py-3">
            {{serie}}
        </div>
    </div>
</template>

<script>
export default {
    name: "CurrentSeriesComponent",
    props : {
        serie: String,
        thumb: String
    }
}
</script>

<style lang="scss" scoped>
    .series_img {
        height: 200px;
        
        img {
            max-height: 100%;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: top;
        }
    }

    .category {
        font-size: 0.85rem
    }
</style>