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

</style>