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

    <div class="footer-nav">
        <div class="container">
            <div class="row">
                <div class="col-6 py-4">
                    <button class="btn btn btn-outline-primary rounded-0 text-white">SIGN-UP NOW!</button>
                </div>
                <div class="col-6">
                    <div class="row py-4">
                        <div class="col-6 d-flex justify-content-end py-3">
                            <h5>FOLLOW US</h5>
                        </div>
                        <div class="col-6 d-flex justify-content-end py-2 justify-content-around">
                            <a href="#"><img src="../assets/footer-facebook.png" alt=""></a>
                            <a href="#"><img src="../assets/footer-twitter.png" alt=""></a>
                            <a href="#"><img src="../assets/footer-youtube.png" alt=""></a>
                            <a href="#"><img src="../assets/footer-pinterest.png" alt=""></a>
                            <a href="#"><img src="../assets/footer-periscope.png" alt=""></a>
                        </div>
                    </div>


                </div>
            </div>
        </div>
    </div>
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

        &:hover {
            color: white;
        }
    }



}

.footer-nav {
    height: 100px;
    background-color: $color-secondary;
    position: relative;
    z-index: 2;

    h5 {
        color: $color-primary;
    }
}
</style>