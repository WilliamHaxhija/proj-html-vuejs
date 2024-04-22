<script>

import PageHero from './PageHero.vue'

export default {
    name: 'PageHeader',
    components: {
        PageHero
    },
    props: {
        navLinks: Array,
        logoImg: String
    },
    methods: {
        getImageUrl(imgName) {
            return new URL(`../assets/img/${imgName}`, import.meta.url).href;
        }
    }
}

</script>

<template>

    <header class="pb-5">

        <nav class="navbar navbar-expand-lg">
            <div class="container">
                <a class="navbar-brand" href="#">
                    <img :src="getImageUrl(logoImg)" :alt="logoImg">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse flex-grow-0" id="navbarNavAltMarkup">
                    <div class="navbar-nav">
                        <a v-for="link in navLinks" class="nav-link ms-link" aria-current="page" href="#">{{ link }}</a>
                        <button class="ms-btn nav-btn">Get a Quote</button>
                    </div>
                </div>
            </div>
        </nav>
        
        <PageHero></PageHero>

        <div>
            <img class="shape" src="../assets/img/bottom-shape.png" alt="shape">
        </div>
    </header>

</template>

<style scoped lang="scss">

@use '../assets/style/generic.scss';

header {
    background-image: url('../assets/img/banner-bg.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: bottom;
    position: relative;


    .ms-link {
        color: white;
    }

    .nav-btn {
        margin-left: 0.8rem;
    }

    .shape {
        max-width: 100%;
        object-fit: contain;
        position: absolute;
        bottom: 0;
        left: 0;
    }
}

@media screen and (max-width: 992px) {

    header {
        .nav-btn {
        margin: 0 auto
    }
    }

}
</style>
