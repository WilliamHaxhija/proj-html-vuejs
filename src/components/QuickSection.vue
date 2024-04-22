<script>

export default {
    name: 'QuickSection'
}

</script>

<template>

    <section class="position-relative">
        <div class="container text-center">
            <h1 class="title mb-5">Anidio Quick Facts</h1>
            <div class="d-flex justify-content-between">
                <div class="card ms-card">
                    <h1>700+</h1>
                    <div>Projects Done</div>
                </div>
                <div class="card ms-card">
                    <h1>250+</h1>
                    <div>Happy Clients</div>
                </div>
                <div class="card ms-card">
                    <h1>25+</h1>
                    <div>Team Members</div>
                </div>
                <div class="card ms-card">
                    <h1>12+</h1>
                    <div>Years on the Market</div>
                </div>
            </div>
        </div>
        <img class="globe" src="../assets/img/globe.png" alt="globe">
        <div>
            <img class="waves bottom" src="../assets/img/shape-bottom.png" alt="waves-bottom">
        </div>
        <div>
            <img class="waves top" src="../assets/img/shape-top.png" alt="waves-top">
        </div>
    </section>

</template>

<style scoped lang="scss">

section {
    background-image: url('../assets/img/counter-bg.png');
    background-repeat: no-repeat;
    background-position: center;
    color: white;
    padding: 5rem;

    .globe {
        position: absolute;
        height: 100%;
        top: 0;
        left: 50%;
        transform: translate(-50%);
    }

    .title {
        font-weight: 700;
        position: relative;
        z-index: 5;
    }

    .ms-card {
        padding: 1.6rem 2.8rem;
        background-color: transparent;
        color: white;
        border-color: white;
        border-radius: 12px;
        z-index: 3;

        div {
            color: #ff7a1f;
        }

        h1 {
            font-weight: 700;
        }
    }

    .waves {
        position: absolute;
        max-width: 100%;
        object-fit: contain;
    }

    .waves.bottom {
        bottom: 0;
        left: 0;
    }

    .waves.top {
        top: 0;
        left: 0;
    }
}

</style>