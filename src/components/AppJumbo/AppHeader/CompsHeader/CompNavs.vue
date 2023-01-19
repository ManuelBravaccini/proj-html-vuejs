<script>
export default {
    name: 'CompNavs',

    data() {
        return {
            navLinks: [
                { name: "Home" },
                { name: "Features" },
                { name: "Achievement" },
                { name: "Blog" },
                { name: "Contact" },
            ]
        }
    },
}

</script>

<template>
    <nav>
        <img src="../../../../assets/imgs/logo.png" alt="Logo Gamer">
        <div>
            <a href="#" v-for="(navLinkEl, index) in navLinks" :key="index">
                {{ navLinkEl.name }}
            </a>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

nav {
    height: 75px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    div {
        display: flex;
        list-style-type: none;

        a {
            text-decoration: none;
            color: $text-color;
            font-weight: 600;
            text-transform: uppercase;
            margin-right: 2rem;
        }
    }
}
</style>