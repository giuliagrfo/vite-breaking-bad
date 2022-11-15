<script>
import { store } from '../store.js/';
import CardsList from './CardsList.vue';
// import SelectorItem from './SelectorItem.vue';
// import axios from 'axios';
export default {
    name: 'AppMain',
    components: {
        CardsList,
        // SelectorItem
    },
    // data() {
    //     return {
    //         store
    //     }
    // },
    // methods: {
    //     // categorySelector() {
    //     //     // console.log('Select');
    //     //     // console.log(this.store.selector);
    //     //     // const url = store.API_URL;

    //     //     const selector = this.store.selector;
    //     //     const url = `${this.store.API_URL}?category=${selector}`;
    //     //     console.log(url);

    //     //     axios.get(url)
    //     //         .then(response => {
    //     //             console.log(response);
    //     //             this.store.characters = response.data
    //     //         })
    //     //         .catch(err => {
    //     //             console.log(err);
    //     //         })
    //     // }
    // }
}
</script>

<template>
    <main id="site_main">
        <div class="container">
            <!-- <SelectorItem @selectCategory="categorySelector" /> -->
            <CardsList />
        </div>
    </main>
</template>


<style lang="scss">
.select {
    width: 300px;
}
</style>