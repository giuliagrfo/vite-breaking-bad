<script>
export default {
    name: 'AppHeader'
}

</script>

<template>
    <header id="site_header">
        <div class="logo">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/77/Breaking_Bad_logo.svg/2560px-Breaking_Bad_logo.svg.png"
                alt="">
            <h1>Breaking Bad Api</h1>
        </div>

    </header>

</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as*;

.logo {
    display: flex;
    margin: 1rem;

    img {
        width: 60px;
        object-fit: contain;
    }

    h1 {
        color: $light;

    }
}
</style>