<script>
import { store } from '../store.js/';

export default {
    name: 'SelectorItem',
    data() {
        return {
            store
        }
    }
}

</script>

<template>
    <select v-model="store.selector" @change="$emit('selectCategory')" class="form-select select">
        <option value="" disabled selected>Select a Tv Series</option>
        <option value="Breaking Bad">Breaking Bad</option>
        <option value="Better Call Saul">Better Call Saul</option>
    </select>
</template>