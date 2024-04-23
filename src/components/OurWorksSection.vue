<script>

export default {
    name: 'OurWorksSection'
}

</script>

<template>

    <section class="ms-padding">

        <div class="container text-center">

            <!-- TITLES -->
            <h4 class="mb-3">Our Works</h4>
            <h1 class="mb-3">Featured Productions</h1>
            <div>Here's just a small sample of some of those projects that we're quite proud of.</div>
            <div>If you're looking for something specific, feel free to get in contact with us.</div>

            <!-- CARDS -->
            <div class="d-flex justify-content-center flex-wrap mt-5">
                <div class="ms-card">
                    <img src="../assets/img/work1.png" alt="work1">
                </div>
                <div class="ms-card">
                    <img src="../assets/img/work2.png" alt="work2">
                </div>
                <div class="ms-card">
                    <img src="../assets/img/work3.png" alt="work3">
                </div>
                <div class="ms-card">
                    <img src="../assets/img/work4.png" alt="work4">
                </div>
            </div>
            <button class="ms-btn border mt-4">See Our Work</button>
        </div>

    </section>

</template>

<style scoped lang="scss">

@use '../style/partials/variables.scss' as *;

h4 {
    color: $brand-primary;
}

.ms-padding {
    padding: 8rem 0;
}

// *****CARDS*****

.ms-card {
    max-width: 45%;
    margin: 1rem;

    &:hover {
        transform: scale(1.05);
        transition: 0.4s;
    }

    img {
        max-width: 100%;
    }
}
</style>