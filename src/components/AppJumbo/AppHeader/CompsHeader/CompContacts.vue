<script>
export default {
    name: 'CompContacts',
}

</script>

<template>
    <section>
        <div>
            <p>+800-123-4567 6587</p>
            <p>Beverly, New York 224 USA</p>
        </div>
        <div>
            <i class="fa-brands fa-facebook-messenger"></i>
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-vimeo-v"></i>
            <i class="fa-brands fa-skype"></i>
            <i class="fa-solid fa-rss"></i>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    display: flex;
    justify-content: space-between;
    align-items: center;

    div {
        display: flex;

        p,
        i {
            padding: 1rem;

        }
    }
}
</style>