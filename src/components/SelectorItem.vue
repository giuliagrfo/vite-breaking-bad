<script>
import { store } from '../store.js/';

export default {
    name: 'SelectorItem',
    emits: ['selectCategory'],

    data() {
        return {
            store
        }
    }
}

</script>

<template>
    <div class="container">
        <select v-model="store.selector" @change="$emit('selectCategory')" class="form-select select">
            <option disabled selected>Select a Tv Series</option>
            <option value="Breaking Bad">Breaking Bad</option>
            <option value="Better Call Saul">Better Call Saul</option>
        </select>
    </div>

</template>