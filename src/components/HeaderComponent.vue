<template>
    <header>
        <nav class="container py-4">
            <div class="row align-items-center gy-4">
                <div class="col-12 col-lg-1 col-xl-2">
                    <img src="@/assets/img/dc-logo.png" alt="logo DC Comics">
                </div>
                <div class="col-12 col-lg-11 col-xl-10 d-flex justify-content-end flex-wrap">
                    <a href="#" v-for="(content, index) in navContent" :key="index" class="text-uppercase">
                        {{ content.categoria }}
                    </a>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>

export default {
    name: 'HeaderComponent',

    data(){
        return {
            navContent: [
                {
                    categoria: "characters",
                    subMenu: ""
                },
                {
                    categoria: "comics",
                    subMenu: ""
                },
                {
                    categoria: "movies",
                    subMenu: ""
                },
                {
                    categoria: "tv",
                    subMenu: ""
                },
                {
                    categoria: "games",
                    subMenu: ""
                },
                {
                    categoria: "collectibles",
                    subMenu: ""
                },
                {
                    categoria: "videos",
                    subMenu: ""
                },
                {
                    categoria: "fans",
                    subMenu: ""
                },
                {
                    categoria: "news",
                    subMenu: ""
                },
                {
                    categoria: "shop",
                    subMenu: ""
                },
            ],
        };
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/variables';

a {
    font-size: 0.85rem;
    font-weight: 600;
    color: $navTextColor;
    padding: 0.75rem 0.75rem 1rem;
    text-decoration: none;

    &.active {
        color: $primaryColor;
    }

    &:hover {
        color: $primaryColor;
    }
}
</style>