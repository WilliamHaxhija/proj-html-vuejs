<script>

export default {
    name: 'PageHero'
}

</script>

<template>

    <!-- HERO CONTAINER -->
    <div class="container-fluid d-flex justify-content-center">
        <div class="text-center mt-3 z">

            <!-- TITLES -->
            <h4 class="mt-5 mb-3">Imagine, Create, Experience</h4>
            <h1>We Animate</h1>
            <h1>With Ninja-Like Precision</h1>
            <div class="mt-3 description">
                We are a character-driven animation studio striving to make high-quality animations.
            </div>
            <div>
                <button class="ms-btn mt-5 me-4">Start a Project</button>
                <button class="ms-btn portfolio-btn mt-5">Portfolio</button>
            </div>
            <!-- BIG HERO IMAGE -->
            <div class="ms-hero-img-ctn">
                <img class="hero" src="../assets/img/middle.png" alt="hero">
                <button class="ms-rounded-btn d-flex justify-content-center align-items-center">
                    <i class="fa-solid fa-play"></i>
                </button>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">

@use '../style/partials/variables.scss' as *;

// *****TITLES*****

* {
    color: white;
}

h1 {
    font-size: 3.9rem;
    font-weight: 700;
}

h4 {
    color: $brand-secondary;
}

.description {
    font-size: 1.2rem;
    font-weight: 300;
}

.portfolio-btn {
    background-color: #270164;
    color: white;

    &:hover {
        transform: scale(1.1);
        transition: 0.2s;
    }
}

.z {
    z-index: 9;
}

// *****HERO IMAGE*****

.ms-hero-img-ctn {
    position: relative;
    margin-top: 5rem;
    margin-bottom: -13rem;
}

.hero {
    z-index: 9;
    width: 100%;

    &:hover {
        transform: scale(1.1);
        transition: 0.5s;
    }
}

// *****BUTTONS*****

.ms-btn {
    box-shadow: 1px 1px 10px rgba(255, 255, 255, 0.356);
}

.ms-rounded-btn {
    width: 50px;
    height: 50px;
    border: none;
    padding: 2.5rem;
    background-color: $brand-primary;
    border-radius: 50px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    i {
        font-size: 1.3rem;
    }

    &:hover {
        background-color: $brand-secondary;
        transition: 0.2s;
    }
}
</style>