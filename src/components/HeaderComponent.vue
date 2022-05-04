<template>
    <header>
        <nav>
            <div class="container">
                <div class="row align-items-center gy-4">
                    <div class="col-12 col-lg-2 col-xl-3 text-center pt-2  text-lg-start p-lg-0">
                        <img src="@/assets/img/dc-logo.png" alt="logo DC Comics">
                    </div>
                    <div class="col-12 col-lg-10 col-xl-9 d-flex justify-content-end flex-wrap gap-3">
                        <a :href="item.href" v-for="item in navContent" :key="item.id" :class="item.categoria === 'comics' ? 'active' : ''" class="text-uppercase">
                            {{ item.categoria }}
                        </a>
                    </div>
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
                    id: 1,
                    href: "#",
                    categoria: "characters",
                },
                {
                    id: 2,
                    href: "#",
                    categoria: "comics",
                },
                {
                    id: 3,
                    href: "#",
                    categoria: "movies",
                },
                {
                    id: 4,
                    href: "#",
                    categoria: "tv",
                },
                {
                    id: 5,
                    href: "#",
                    categoria: "games",
                },
                {
                    id: 6,
                    href: "#",
                    categoria: "collectibles",
                },
                {
                    id: 7,
                    href: "#",
                    categoria: "videos",
                },
                {
                    id: 8,
                    href: "#",
                    categoria: "fans",
                },
                {
                    id: 9,
                    href: "#",
                    categoria: "news",
                },
                {
                    id: 10,
                    href: "#",
                    categoria: "shop",
                },
            ],
        };
    }
}
</script>

<style lang="scss" scoped>


nav {

    a { 
    font-size: 0.85rem;
    font-weight: 600;
    color: $navTextColor;
    display: inline-block;
    padding: 2.8rem 0;
    border-bottom: 7px solid transparent;
    text-decoration: none;

        &.active {
            color: $primaryColor;
        }

        &:hover {
            color: $primaryColor;
            border-bottom: 7px solid $primaryColor;
        }
    }
}
</style>