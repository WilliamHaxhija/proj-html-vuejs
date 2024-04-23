<script>

export default {
    name: 'OurProcessSection'
}

</script>

<template>

    <section class="position-relative">
        <div class="container">
            <div class="titles-ctn position-relative ms-auto">
                <h4 class="mb-4">Our Process</h4>
                <h1>Our Process for</h1>
                <h1>Your Animation</h1>
                <h1>Production</h1>
                <div class="mt-4 mb-5">We have an effective process for working on animation.</div>
                <div class="ms-card-ctn d-flex justify-content-start">
                    <div class="card border ms-card card-3 position relative text-center">
                        <div class="img-ctn mb-3">
                            <img src="../assets/img/process2.png" alt="process2">
                        </div>
                        <h3 class="mb-2">Pre-Production</h3>
                        <p>We'll take your ideas and create a technical script which consists of action notes and
                            animation descriptions.</p>
                        <span class="pb-2">4</span>
                    </div>
                    <div class="card border ms-card card-3 position relative text-center ms-4">
                        <div class="img-ctn mb-3">
                            <img src="../assets/img/process1.png" alt="process1">
                        </div>
                        <h3 class="mb-2">Scripting</h3>
                        <p>We'll take your ideas and create a technical script which consists of action notes and
                            animation descriptions.</p>
                        <span class="pb-2">1</span>
                    </div>
                </div>
                <div class="ms-3">
                    <button class="ms-btn arrow-btn position-relative border mt-4 me-3"><i
                            class="fa-solid fa-arrow-left"></i></button>
                    <button class="ms-btn arrow-btn position-relative border mt-4"><i
                            class="fa-solid fa-arrow-right"></i></button>
                </div>
            </div>
        </div>
        <img class="big-img" src="../assets/img/process-thumb.png" alt="process">
        <img class="space-ship" src="../assets/img/smart4.png" alt="smart4">
    </section>

</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

h4 {
    color: $brand-primary;
}

.titles-ctn {
    max-width: 48%;
}

.big-img {
    width: 750px;
    position: absolute;
    top: 0;
    left: -190px;
    z-index: -1;
}

.ms-card {
    max-width: 50%;
    border-radius: 25px;
    padding: 1.5rem 1rem;

    &:hover {
        background-image: linear-gradient(white, #fff3ea);
        border: 2px solid white;
        transition: 0.5s;
    }

    .img-ctn {
        width: 110px;
        height: 100px;
        background-color: #fef5f0;
        border-radius: 50px;
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 auto;
    }

    img {
        margin: 0 auto 1rem auto;
        width: 50%;
    }

    h3 {
        font-weight: 600;
    }

    span {
        background-color: #f7f0ff;
        width: 40px;
        height: 100px;
        border-bottom-left-radius: 30px;
        border-bottom-right-radius: 30px;
        position: absolute;
        top: 0;
        right: 20px;
        display: flex;
        align-items: end;
        justify-content: center;
    }

}

.space-ship {
    position: absolute;
    width: 90px;
    bottom: -105px;
    right: 0;
}
</style>