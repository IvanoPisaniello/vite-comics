<script>
export default {
    components: {
        name: 'Card',
    },

    props: {
        thumb: String,
        price: String,

    }





}
</script>

<template>
    <div class="card text-start">
        <img class="card-img-top" :src="thumb" alt="Title">
        <div class="card-body">
            <h4 class="card-title">Title</h4>
            <p class="card-text">Body</p>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

.main-container {
    height: 500px;
    background-color: $color-tertiary;

    .card {
        width: 100px;
        height: 150px;
    }

}
</style>