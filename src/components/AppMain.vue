<script>
import CardsList from './CardsList.vue';

export default {
    name: 'AppMain',
    components: {
        CardsList,
    }
}
</script>

<template>
    <main id="site_main">
        <div class="container">
            <CardsList />
        </div>
    </main>
</template>


<style lang="scss">
.select {
    width: 300px;
}
</style>