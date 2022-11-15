<script>
import CardsList from './CardsList.vue';
import SelectorItem from './SelectorItem.vue';

export default {
    name: 'AppMain',
    components: {
        CardsList,
        SelectorItem
    }
}
</script>

<template>
    <main id="site_main">
        <div class="container">
            <!-- <div class="dropdown">
                <button class="btn btn-light dropdown-toggle" type="button" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Select Category
                </button>
                <div class="dropdown-menu">
                    <button class="dropdown-item" href="#">Action</button>
                    <button class="dropdown-item" href="#">Action</button>
                </div>
            </div> -->
            <SelectorItem />
            <CardsList />
        </div>
    </main>
</template>


<style lang="scss">
.select {
    width: 300px;
}
</style>