<script>
import { store } from '../store.js';

export default {
    name: 'ResultsItem',
    data() {
        return {
            store
        }
    },
    computed: {
        finalResult() {
            return this.store.characters.length
        }
    }
}

</script>

<template>
    <div class="results">
        <p v-if="store.characters !== null">Results: {{ finalResult }}</p>
    </div>

</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as*;

.results {
    background-color: $dark;
    padding: 1rem;
    margin: 1rem 0;
    color: $light;

    p {
        margin: 0;
    }
}
</style>