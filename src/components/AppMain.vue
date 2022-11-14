<script>
export default {
    name: 'AppMain'
}

</script>

<template>
    <main id="site_main">
        <div class="container">
            <div class="dropdown">
                <button class="btn btn-light dropdown-toggle" type="button" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Dropdown Button
                </button>
                <div class="dropdown-menu">
                    <button class="dropdown-item" href="#">Action</button>
                    <button class="dropdown-item" href="#">Action</button>
                </div>
            </div>
            <div class="characters">
                <div class="container">
                    <div class="found_characters">
                        <h6>Found 62 characters</h6>
                    </div>
                    <div class="row list row-cols-5">
                        <div class="card">
                            <div class="col">
                                <img src="https://images.amcnetworks.com/amc.com/wp-content/uploads/2015/04/cast_bb_700x1000_walter-white-lg.jpg"
                                    alt="">
                                <h4>Walter White</h4>
                                <h5>Breaking bad</h5>
                                <h6>Dead</h6>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>


    </main>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as*;

.characters {
    background-color: $light;
    padding: 2rem;
    margin-top: 1rem;

    .found_characters {
        background-color: $dark;
        padding: 1rem;
        margin: 1rem 0;
        color: $light;
    }

    .list {
        padding: 2rem;
    }

    .card {
        background-color: $primary;
        border-radius: 0;
        padding: 1rem;
        text-align: center;

        h4 {
            color: $light;
            text-transform: uppercase;
            margin: 1rem 0;
        }

        h5 {
            color: $soft;
        }

        h6 {
            color: $soft;
        }
    }


}
</style>