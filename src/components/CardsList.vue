<script>
import CardItem from './CardItem.vue';
import { store } from '../store.js'

export default {
    name: 'CardsList',
    components: {
        CardItem
    },
    data() {
        return {
            store
        }
    }
}

</script>

<template>
    <div class="characters">
        <div class="container">
            <div class="found_characters">
                <h6>Found 62 characters</h6>
            </div>
            <div class="row list row-cols-5">
                <CardItem :character="character" v-for="character in store.characters" />
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as*;

.characters {
    background-color: $light;
    padding: 2rem;
    margin-top: 1rem;

    .found_characters {
        background-color: $dark;
        padding: 1rem;
        margin: 1rem 0;
        color: $light;

        h6 {
            margin: 0;
        }
    }

    .list {
        justify-content: center;
    }
}
</style>