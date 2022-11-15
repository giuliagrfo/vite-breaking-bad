<script>
import axios from 'axios';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import SelectorItem from './components/SelectorItem.vue';
import { store } from './store.js';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    SelectorItem,
  },
  data() {
    return {
      store
    }
  },
  methods: {
    // callApi(url) {
    //   axios.get(url)
    //     .then(response => {
    //       console.log(response);
    //       this.store.characters = response.data
    //     })
    // },
    categorySelector() {
      // console.log('Select');
      // console.log(this.store.selector);
      // const url = store.API_URL;

      const selector = this.store.selector;
      const url = `${this.store.API_URL}?category=${selector}`;
      console.log(url);

      axios.get(url)
        .then(response => {
          console.log(response);
          this.store.characters = response.data
        })
        .catch(err => {
          console.log(err);
        })
    }
  },
  mounted() {
    this.categorySelector(this.store.API_URL)
  }
}

</script>

<template>
  <AppHeader />
  <SelectorItem @selectCategory="categorySelector" />
  <AppMain />

</template>

