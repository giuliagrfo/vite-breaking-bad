<script>
export default {
    name: 'SelectorItem'
}

</script>

<template>
    <select v-model="categorySelector" @change="" class="form-select select">
        <option value="" disabled selected>Select a Tv Series</option>
        <option value="Breaking Bad">Breaking Bad</option>
        <option value="Better Call Saul">Better Call Saul</option>
    </select>
</template>