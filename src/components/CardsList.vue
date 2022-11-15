<script>
import CardItem from './CardItem.vue';
import ResultsItem from './ResultsItem.vue';

import { store } from '../store.js'

export default {
    name: 'CardsList',
    components: {
        CardItem,
        ResultsItem
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

            <ResultsItem />

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

    .list {
        justify-content: center;
    }
}
</style>