<script>

export default {
    name: 'PageFooter',
    props: {
        links: Array,
        logoImg: String
    },
    methods: {
        getImageUrl(string) {
            return new URL(`../assets/img/${string}`, import.meta.url).href;
        }
    }
}

</script>

<template>

    <footer class="pb-4 position-relative">
        <div class="container">
            <div class="d-flex align-items-center justify-content-between">
                <div class="logo">
                    <img :src="getImageUrl(logoImg)" :alt="logoImg">
                </div>
                <div class="links">
                    <a class="mx-3" v-for="link in links" href="#">{{ link }}</a>
                </div>
            </div>
            <hr>
            <div class="container d-flex align-items-center justify-content-between">
                <div class="d-flex align-items-center">
                    Copyright @ 2022 <a class="softvius" href="#">Softvius</a>. All rights reserved.
                </div>
                <div class="socials d-flex">
                    <div class="d-flex align-items-center justify-content-center"><i class="fa-brands fa-facebook-f"></i></div>
                    <div class="d-flex align-items-center justify-content-center"><i class="fa-brands fa-twitter"></i></div>
                    <div class="d-flex align-items-center justify-content-center"><i class="fa-brands fa-instagram"></i></div>
                </div>
            </div>
        </div>
        <div class="footer-btn d-flex align-items-center justify-content-center">
            <i class="fa-solid fa-arrow-up"></i>
        </div>
    </footer>

</template>

<style scoped lang="scss">

@use '../style/partials/variables.scss' as *;

.logo {
    filter: invert(1);
}

a {
    text-decoration: none;
    color: black;
    font-weight: 600;

    &:hover {
        color: $brand-primary;
        transition: 0.2s;
    }
}

.softvius {
    color: $brand-primary;
    margin-left: 0.3rem;

    &:hover {
        color: black;
        transition: 0.2s;
    }
}

.socials {
    div {
        width: 40px;
        height: 40px;
        padding: 8px;
        border: 1px solid lightgrey;
        border-radius: 50px;
        margin: 0 0.3rem;
        background-color: white;
        color: $brand-primary;
        cursor: pointer;

        &:hover {
            background-color: $brand-secondary;
            color: white;
            transition: 0.2s;
        }
    }
}

.footer-btn {
    width: 40px;
    height: 40px;
    background-color: #270164;
    color: white;
    border-radius: 5px;
    padding: 8px;
    cursor: pointer;
    position: absolute;
    bottom: 15px;
    right: 15px;

    &:hover {
        background-color: $brand-secondary;
    }
}
</style>
