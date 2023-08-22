<script>
export default {
    components: {
        name: 'TheHeader',
    },
    data() {
        return {
            navLinks: [
                { name: "Caracters", path: "/" },
                { name: "Comics", path: "/products" },
                { name: "Movies", path: "/contacts" },
                { name: "Games", path: "/about" },
                { name: "Collectibles", path: "/about" },
                { name: "Videos", path: "/about" },
                { name: "Fans", path: "/about" },
                { name: "News", path: "/about" },
                { name: "Shop", path: "/about" },

            ],
        };
    },
}
</script>

<template>
    <div class="navbar container">
        <img src="../assets/dc-logo.png" alt="" class="logo-image">

        <ul class="nav nav-underline">

            <li class="nav-item" v-for="link in navLinks">
                <a class="nav-link pb-4" href="#">{{ link.name }}</a>
            </li>

        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.navbar {
    height: 80px;


    .logo-image {
        height: 60px;
    }

    .nav-link {
        color: black;

        &:hover {
            color: $color-primary;
        }
    }
}
</style>