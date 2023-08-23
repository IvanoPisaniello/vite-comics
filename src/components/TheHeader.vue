<script>
export default {
    components: {
        name: 'TheHeader',
    },
    data() {
        return {
            navLinks: [
                { name: "CARACTERS", path: "/" },
                { name: "COMICS", path: "/products" },
                { name: "MOVIES", path: "/contacts" },
                { name: "GAMES", path: "/about" },
                { name: "COLLECTIBLES", path: "/about" },
                { name: "VIDEOS", path: "/about" },
                { name: "FANS", path: "/about" },
                { name: "NEWS", path: "/about" },
                { name: "SHOP", path: "/about" },

            ],
        };
    },
}
</script>

<template>
    <div class="navbar container">
        <img src="../assets/dc-logo.png" alt="" class="logo-image">

        <ul class="nav nav-underline">

            <li class="nav-item " v-for="link in navLinks">
                <a class="nav-link pb-4" href="#">{{ link.name }}</a>
            </li>

        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.navbar {
    height: 62px;
    width: 900px;


    .logo-image {
        height: 50px;
    }

    .nav-link {
        color: black;
        font-size: .8rem;

        &:hover {
            color: $color-primary;
        }
    }
}
</style>