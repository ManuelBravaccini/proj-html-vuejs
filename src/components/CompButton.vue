<script>
export default {
    name: 'CompButton',
}
</script>

<template>
    <button>

    </button>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

button {
    padding: 1rem;
    font-weight: bold;
    text-transform: uppercase;
    color: $secondary-color;
    background-color: $text-color;
    border-radius: 5px;
}
</style>