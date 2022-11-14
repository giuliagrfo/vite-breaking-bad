<script>
export default {
    name: 'CardItem',
    props: {
        character: Object
    }
}
</script>

<template>
    <div class="card">
        <div class="col">
            <img :src="character.img" :alt="character.name">
            <h4>{{ character.name }}</h4>
            <h5>{{ character.category }}</h5>
            <h6>{{ character.status }}</h6>
        </div>
    </div>


</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as*;



.card {
    background-color: $primary;
    border-radius: 0;
    padding: 1rem;
    text-align: center;
    margin: 1rem;

    h4 {
        color: $light;
        text-transform: uppercase;
        margin: 1rem 0;
    }

    h5 {
        color: $soft;
    }

    h6 {
        color: $soft;
    }
}
</style>