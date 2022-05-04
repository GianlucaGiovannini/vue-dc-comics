<template>
    <div class="footer_top position-relative">
        <div class="container">
            <div class="row row-cols-1 row-cols-sm-2">
                <div class="col footer_list py-4">
                    <div class="row row-cols-3">
                        <div class="col" v-for="({titles, links}, index) in footerMenu" :key="index" :class="footerMenu.length -1 === index ? 'm_t_negativo': '' ">
                            <h4 class="text-white py-2">{{titles}}</h4>
                            <ul>
                                <li v-for="(link,index) in links" :key="index">
                                    <a :href="link.href">{{link.text}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>   
</template>

<script>
export default {
    name: "FooterTopComponent",

    data() {
        return {
            footerMenu: [
                {
                    titles: "DC Comics",
                    links: [
                        {
                            href: "#",
                            text: "Characters",
                        },
                        {
                            href: "#",
                            text: "Comics",
                        },
                        {
                            href: "#",
                            text: "Movie",
                        },
                        {
                            href: "#",
                            text: "TV",
                        },
                        {
                            href: "#",
                            text: "Games",
                        },
                        {
                            href: "#",
                            text: "Videos",
                        },
                        {
                            href: "#",
                            text: "News",
                        }
                    ]
                },
                {
                    titles: "DC",
                    links: [
                        {
                            href: "#",
                            text: "Terms of Use",
                        },
                        {
                            href: "#",
                            text: "Privacy policy (New)",
                        },
                        {
                            href: "#",
                            text: "Ad Choise",
                        },
                        {
                            href: "#",
                            text: "Advertising",
                        },
                        {
                            href: "#",
                            text: "Jobs",
                        },
                        {
                            href: "#",
                            text: "Subscription",
                        },
                        {
                            href: "#",
                            text: "Talent Workshops",
                        },
                        {
                            href: "#",
                            text: "CPSC Certificates",
                        },
                        {
                            href: "#",
                            text: "Rating",
                        },
                        {
                            href: "#",
                            text: "Shop Help",
                        },
                        {
                            href: "#",
                            text: "Contact Us",
                        }
                    ]
                },
                {
                    titles: "Sites",
                    links: [
                        {
                            href: "#",
                            text: "DC",
                        },
                        {
                            href: "#",
                            text: "MAD Magazine",
                        },
                        {
                            href: "#",
                            text: "DC Kids",
                        },
                        {
                            href: "#",
                            text: "DC Universe",
                        },
                        {
                            href: "#",
                            text: "DC Power Visa",
                        }
                    ]
                },
                {
                    titles: "Shop",
                    links: [
                        {
                            href: "#",
                            text: "Shop DC",
                        },
                        {
                            href: "#",
                            text: "Shop DC Collectibles",
                        }
                    ]
                }
            ]
        };
    }
}
</script>

<style lang="scss" scoped>
 
</style>