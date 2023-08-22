<script>
export default {
    components: {
        name: 'TheMain',
    }
}
</script>

<template>
    <div class="main-container py-4">
        <div class="container">
            <h4 class="text-light "> -- Content goes here -- </h4>
        </div>
        <div class="card-container">

        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

.main-container {
    height: 100px;
    background-color: $color-tertiary;

}
</style>