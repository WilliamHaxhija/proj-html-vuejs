<script>

//*****COMPONENTS*****

import PageHero from './PageHero.vue'

export default {
    name: 'PageHeader',
    components: {
        PageHero
    },

    //*****PROPS*****
    props: {
        navLinks: Array,
        logoImg: String
    },

    //*****DATA*****
    data () {
        return {
            activeLink: 1
        }
    },

    //*****METHODS*****
    methods: {
        getImageUrl(imgName) {
            return new URL(`../assets/img/${imgName}`, import.meta.url).href;
        },
        activateLink(number) {
            this.activeLink = number;
        }
    }
}

</script>

<template>

    <header class="pb-5">

        <!-- NAVBAR -->
        <nav class="navbar navbar-expand-lg pt-3 z">
            <div class="container">
                <a class="navbar-brand" href="#">
                    <!-- DYANAMIC LOGO -->
                    <img :src="getImageUrl(logoImg)" :alt="logoImg">
                </a>
                <button class="navbar-toggler burger" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon burger-icon"></span>
                </button>
                <div class="collapse navbar-collapse flex-grow-0" id="navbarNavAltMarkup">
                    <div class="navbar-nav">
                        <!-- DYNAMIC LINKS -->
                        <a v-for="link, index in navLinks" :class="{msactive: activeLink === index}" class="nav-link ms-link me-3" aria-current="page" href="#" @click="activateLink(index)">{{ link }}</a>
                        <button class="ms-btn nav-btn">Get a Quote</button>
                    </div>
                </div>
            </div>
        </nav>

        <!-- HEADER IMAGES -->
        <img class="globe3" src="../assets/img/globe3.png" alt="globe3">
        <img class="globe2" src="../assets/img/globe2.png" alt="globe2">
        <img class="globe1" src="../assets/img/globe1.png" alt="globe1">
        <img class="ufo" src="../assets/img/light.png" alt="ufo">
        <img class="dots dots-left" src="../assets/img/dots-left.png" alt="dots">
        <img class="dots dots-right" src="../assets/img/dots-right.png" alt="dots">
        <img class="astronaut astronaut-left" src="../assets/img/left-man.png" alt="astronaut">
        <img class="astronaut astronaut-rigth" src="../assets/img/right-man.png" alt="astronaut">

        <!-- HERO -->
        <PageHero></PageHero>

        <!-- WAVES IMAGES -->
        <div>
            <img class="shape" src="../assets/img/bottom-shape.png" alt="shape">
        </div>
    </header>

</template>

<style scoped lang="scss">

@use '../style/partials/variables.scss' as *;

//*****HEADER*****

header {
    background-image: url('../assets/img/banner-bg.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: bottom;
    position: relative;

    .ms-link,
    .burger {
        color: white;
    }

    .ms-link:hover {
        color: #ff7a1f;
        transition: 0.2s;
    }

    .msactive {
        color: $brand-secondary !important;
    }

    .burger-icon {
        filter: invert(1);
    } 

    .nav-btn {
        margin-left: 0.8rem;
    }

    //*****HERO*****

    .shape {
        max-width: 100%;
        object-fit: contain;
        position: absolute;
        bottom: 0;
        left: 0;
    }

    //*****IMAGES*****

    .astronaut {
        max-width: 200px;
        position: absolute;
        top: 23%;
    }

    .astronaut-left {
        left: 2px;
    }

    .astronaut-rigth {
        right: 2px;
    }

    .dots {
        position: absolute;
        width: 50%;
    }

    .dots-right {
        right: 0;
    }

    .dots-left {
        left: 50px;
    }

    .globe1 {
        width: 100px;
        position: absolute;
        top: 100px;
        left: 130px;
    }

    .globe2 {
        width: 81px;
        position: absolute;
        top: 150px;
        right: 350px;
    }

    .globe3 {
        width: 220px;
        position: absolute;
        top: -130px;
        left: 35%;
    }

    .ufo {
        width: 100px;
        position: absolute;
        right: 100px;
    }

    .z {
        z-index: 9;
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
