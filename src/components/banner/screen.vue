<template>
    <div id="app">

        <div class="py-5">
            <div class="container-fluid">
                <div class="row">
                    <div class="col-md-12">
                        <img class="img-fluid d-block mx-auto logo" src="assets/images/open-infrastructure-logo.svg">
                    </div>
                </div>
            </div>
        </div>

        <banner :banner="banner.state.static_banner"></banner>
    </div>
</template>

<script>

    import Banner from './banner.vue'
    import { mapGetters } from 'vuex'

    export default {
        computed: {
            ...mapGetters({
                banner: 'banner'
            }),
        },
        components: { Banner }
    }

</script>

<style>

    .logo {
        width: 80%;
    }

</style>
