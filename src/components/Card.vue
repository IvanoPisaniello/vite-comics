<script>
export default {
    components: {
        name: 'Card',
    },

    props: {
        thumb: String,
        price: String,
        series: String,

    }





}
</script>

<template>
    <div class="single-card text-start">
        <div class="img-container">
            <a href="#"><img class="card-img-top img-card" :src="thumb" alt="Title"></a>
        </div>
        <div class="">
            <p class="text-light text-center">{{ series }}</p>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;





.img-card {
    height: 120px;
}

// .img-container {
//     height: 120px;
//     overflow: hidden;
// }

p {
    font-size: .8rem;
}
</style>