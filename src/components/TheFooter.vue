<script>
export default {
    components: {
        name: 'TheFooter',
    },

    data() {
        return {
            DcComicsLinks: [
                { name: "Caracters" },
                { name: "Comics" },
                { name: "Movies" },
                { name: "Games" },
                { name: "Collectibles", },
                { name: "Videos", },
                { name: "Fans", },
                { name: "News", },

            ],
            shopLinks: [
                { name: "Shop DC" },
                { name: "Shop DC Collectibles" },


            ],
            DcLinks: [
                { name: "Term Of Use" },
                { name: "Privacy policy (New)" },
                { name: "Ad Choices" },
                { name: "Advertsing" },
                { name: "Subscriptions", },
                { name: "Talent Workshops", },
                { name: "Ratings", },
                { name: "Shop Help", },
                { name: "Contact Us", },



            ],
            SitesLinks: [
                { name: "DC" },
                { name: "Mad Magazine" },
                { name: "DC Kids" },
                { name: "DC Universe" },
                { name: "DC Power Visa", },



            ],
        };
    },
}
</script>

<template>
    <div class="list-container">
        <div class="container">
            <div class="row p-4">
                <div class="col-5">
                    <div class="row">
                        <div class="col-4">
                            <p class="text-light">DC COMICS</p>
                            <ul class="p-0">
                                <li v-for="link in DcComicsLinks" class="list-unstyled"> <a href="#">{{
                                    link.name }}</a>
                                </li>
                            </ul>
                            <p class="text-light">SHOP</p>
                            <ul class="p-0">
                                <li v-for="link in shopLinks" class="list-unstyled"> <a href="#">{{
                                    link.name }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <p class="text-light">DC</p>
                            <ul class="p-0">
                                <li v-for="link in DcLinks" class="list-unstyled"> <a href="#">{{
                                    link.name }}</a>
                                </li>
                            </ul>

                        </div>
                        <div class="col-4">
                            <p class="text-light">SITES</p>
                            <ul class="p-0">
                                <li v-for="link in SitesLinks" class="list-unstyled"> <a href="#">{{
                                    link.name }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-7">
                    <img src="../assets/dc-logo-bg.png" alt="" class="bg-logo">
                </div>
            </div>
        </div>
    </div>

    <div class="footer-nav"></div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.list-container {
    height: 400px;
    background-image: url(../assets/footer-bg.jpg);
    position: relative;



    .bg-logo {
        position: absolute;
        right: 50px;
        bottom: -60px;
        height: 600px;
        width: 600px;
    }

    a {
        text-decoration: none;
        font-size: .8rem;
        color: $color-list;
    }



}

.footer-nav {
    height: 100px;
    background-color: $color-secondary;
    position: relative;
    z-index: 2;
}
</style>