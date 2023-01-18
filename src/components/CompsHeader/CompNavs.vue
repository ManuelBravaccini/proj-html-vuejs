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
        <ul>
            <li v-for="(navLinkEl, index) in navLinks" :key="index">
                {{ navLinkEl.name }}
            </li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
ul {
    display: flex;
    list-style-type: none;
}
</style>