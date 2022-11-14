<script>
import CardsList from './CardsList.vue';
export default {
    name: 'AppMain',
    components: {
        CardsList
    }
}
</script>

<template>
    <main id="site_main">
        <div class="container">
            <div class="dropdown">
                <button class="btn btn-light dropdown-toggle" type="button" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Select Category
                </button>
                <div class="dropdown-menu">
                    <button class="dropdown-item" href="#">Action</button>
                    <button class="dropdown-item" href="#">Action</button>
                </div>
            </div>
            <CardsList />
        </div>
    </main>
</template>
