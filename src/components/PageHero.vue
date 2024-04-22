<script>

    export default {
        name: 'PageHero'
    }

</script>

<template>

    <div class="container-fluid d-flex justify-content-center">
        <div class="text-center">
            <h4 class="mt-5 mb-3">Imagine, Create, Experience</h4>
            <h1>We Animate</h1>
            <h1>With Ninja-Like Precision</h1>
            <h5 class="mt-3">We are character-driven animation studio striving to make high-quality animations.</h5>
            <div>
                <button class="ms-btn mt-4 me-4">Start a Project</button>
                <button class="ms-btn portfolio-btn mt-4">Portfolio</button>
            </div>
            <img class="mt-5 hero" src="../assets/img/middle.png" alt="hero">
        </div>
    </div>

</template>

<style scoped lang="scss">

@use '../assets/style/generic.scss';

* {
    color: white;
}

h1 {
    font-size: 4rem;
    font-weight: 600;
}

h4 {
    color: #ff7a1f;
}

.portfolio-btn {
    background-color: #270164;
    color: white;
    border: 1px solid white;
}

.hero {
    z-index: 9;
    position: relative;
    margin-bottom: -13rem;
}

</style>