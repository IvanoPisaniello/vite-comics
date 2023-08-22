<script>
export default {
    components: {
        name: 'CardContainer',
    }
}
</script>

<template>
    <div class="card-container">
        <div class="container d-flex justify-content-around align-items-center py-5">

            <div class="d-flex ">
                <img src="../assets/buy-comics-digital-comics.png" alt="">
                <p class="text-white p-2">DIGITAL COMICS</p>
            </div>
            <div class="d-flex ">
                <img src="../assets/buy-comics-merchandise.png" alt="">
                <p class="text-white p-2">DC MERCIANDISE</p>
            </div>
            <div class="d-flex ">
                <img src="../assets/buy-comics-subscriptions.png" alt="">
                <p class="text-white p-2">SUBSCRIPTION</p>
            </div>
            <div class="d-flex ">
                <img src="../assets/buy-comics-shop-locator.png" alt="">
                <p class="text-white p-2">COMIC SHOP LOCATOR</p>
            </div>
            <div class="d-flex ">
                <img src="../assets/buy-dc-power-visa.svg" alt="">
                <p class="text-white p-2">DC POWER VISA</p>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

.card-container {
    height: 150px;
    background-color: $color-primary;
    position: relative;
    z-index: 1;

    img {
        height: 50px;
    }
}
</style>