<script>

export default {
    name: 'FirstSection'
}

</script>

<template>

    <section class="ms-margin position-relative">

        <div class="container-fluid position-relative text-center">

            <!-- TITLES -->
            <div class="titles">
                <h4>Our Love For Animation</h4>
                <h1>We're Storytelling</h1>
                <h1>Experts With Creative</h1>
                <h1>Smarts</h1>
                <div>
                    Our culture inspires the creative and innovative spirit found throughout our Studio. We breathe life
                    into new ideas!
                </div>
            </div>

            <!-- CARDS -->
            <img class="big-img" src="../assets/img/smart.png" alt="smart">
            <div class="container mt-5 d-flex ms-padding justify-content-end">
                <div class="card ms-card card-1">
                    <img src="../assets/img/smart1.png" alt="search">
                    <h3>3D Modeling</h3>
                    <p>We constantly ask questions. It helps us shape your story and deliver the results you crave. Yep,
                        we'll drill deep to deliver above and beyond your expectations.</p>
                </div>
                <div class="card ms-card card-2 ms-4">
                    <img src="../assets/img/smart2.png" alt="smart2">
                    <h3>Collaboration</h3>
                    <p>We constantly ask questions. It helps us shape your story and deliver the results you crave. Yep,
                        we'll drill deep to deliver above and beyond your expectations.</p>
                </div>
                <div class="card ms-card card-3 position relative ms-4">
                    <img src="../assets/img/smart3.png" alt="brain-light">
                    <h3 class="mb-2">Creativity</h3>
                    <p>We constantly ask questions. It helps us shape your story and deliver the results you crave. Yep,
                        we'll drill deep to deliver above and beyond your expectations.</p>
                </div>
            </div>
        </div>
        <img class="space-ship" src="../assets/img/smart4.png" alt="smart4">

    </section>

</template>

<style scoped lang="scss">

@use '../style/partials/variables.scss' as *;

.ms-margin {
    margin-top: 17rem;
}

.ms-padding {
    padding-bottom: 7rem;
}

// *****TITLES*****

.titles {
    max-width: 50%;
    margin: 0 auto;

    h1 {
        font-size: 3rem;
        font-weight: 600;
    }

    h4 {
        color: $brand-primary;
    }
}

.big-img {
    width: 400px;
    height: 800px;
    position: absolute;
    left: 0;
    top: -100px;
    z-index: -1;
}

// *****CARDS*****

.ms-card {
    max-width: 25%;
    border-radius: 35px;
    padding: 1.5rem 1rem;

    img {
        margin: 0 auto 1rem auto;
        width: 32%;
    }

    h3 {
        font-weight: 600;
    }
}

.card-1 {
    background-image: linear-gradient(white, #fff3ea);

    &:hover {
        background-image: linear-gradient(#fff3ea, white);
        border: 2px solid white;
        transition: 0.5s;
    }
}

.card-2 {
    background-image: linear-gradient(white, #eeebfc);

    &:hover {
        background-image: linear-gradient(#eeebfc, white);
        border: 2px solid white;
        transition: 0.5s;
    }
}

.card-3 {
    background-image: linear-gradient(white, #ffe7e7);

    &:hover {
        background-image: linear-gradient(#ffe7e7, white);
        border: 2px solid white;
        transition: 0.5s;
    }
}

.space-ship {
    position: absolute;
    width: 90px;
    bottom: 0;
    right: 0;
}
</style>