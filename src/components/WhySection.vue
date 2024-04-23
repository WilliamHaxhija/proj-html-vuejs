<script>

export default {
    name: 'WhySection'
}

</script>

<template>

    <section class="my-5 py-5">
        <div class="container">
            <div class="titles w-50 text-center mt-5 pt-5 mx-auto">
                <h4>Why Anidio Studio?</h4>
                <h1>We Love Our Clients</h1>
                <div>We're trusted throughout adiand and have a wealth of recommendations from start-ups to renowned global brands.</div>
            </div>
            <div class="ms-cards-ctn mt-5 d-flex justify-content-center">
                <div class="card ms-card mt-2 mx-2">
                    <img src="../assets/img/sponsor5.png" alt="pillar">
                </div>
                <div class="card ms-card mt-2 mx-2">
                    <img src="../assets/img/sponsor6.png" alt="digital-eagle">
                </div>
                <div class="card ms-card mt-2 mx-2">
                    <img src="../assets/img/sponsor1.png" alt="supreme">
                </div>
                <div class="card ms-card mt-2 mx-2">
                    <img src="../assets/img/sponsor2.png" alt="phoenix">
                </div>
                <div class="card ms-card mt-2 mx-2">
                    <img src="../assets/img/sponsor3.png" alt="cooperation">
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped lang="scss">

@use '../style/partials/variables.scss' as *;

h4 {
    color: $brand-primary;
}

.ms-card {
    border: none;

    &:hover {
        filter: invert(1);
        transform: scale(1.1);
        transition: 0.5s;
    }
}

</style>
