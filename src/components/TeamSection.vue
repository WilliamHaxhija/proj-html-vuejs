<script>

export default {
    name: 'TeamSection'
}

</script>

<template>
    <section class="ms-margin position-relative">
        <div class="container text-center">
            <div class="titles w-50 mx-auto">
                <h4 class="mb-3">Audio Magic Team Member</h4>
                <h1>Let Us Animate Your</h1>
                <h1 class="mb-3">Project</h1>
                <div>We create new wolrds! Let's collaborate and create engaging, effective, award-winning animations.
                </div>
            </div>
            <div class="ms-card-ctn d-flex flex-nowrap justify-content-center mt-5">
                <div class="card ms-card">
                    <img src="../assets/img/team1.png" alt="robert-coleman">
                    <h4 class="text-dark mt-5">Robert Coleman</h4>
                    <div class="mt-3">Owner & Creative Director</div>
                    <div class="card-social d-flex mt-5 mb-4 mx-auto">
                        <div><i class="fa-brands fa-facebook-f"></i></div>
                        <div><i class="fa-brands fa-twitter"></i></div>
                        <div><i class="fa-brands fa-instagram"></i></div>
                    </div>
                </div>
                <div class="card ms-card">
                    <img src="../assets/img/team2.png" alt="don-woods">
                    <h4 class="text-dark mt-5">Don Woods</h4>
                    <div class="mt-3">Administrator</div>
                    <div class="card-social d-flex mt-5 mb-4 mx-auto">
                        <div><i class="fa-brands fa-facebook-f"></i></div>
                        <div><i class="fa-brands fa-twitter"></i></div>
                        <div><i class="fa-brands fa-instagram"></i></div>
                    </div>
                </div>
                <div class="card ms-card">
                    <img src="../assets/img/team4.png" alt="tomas-nash">
                    <h4 class="text-dark mt-5">Tomas Nash</h4>
                    <div class="mt-3">2D Animator & Compositor"</div>
                    <div class="card-social d-flex mt-5 mb-4 mx-auto">
                        <div><i class="fa-brands fa-facebook-f"></i></div>
                        <div><i class="fa-brands fa-twitter"></i></div>
                        <div><i class="fa-brands fa-instagram"></i></div>
                    </div>
                </div>
            </div>
            <div class="ms-btn-ctn mt-3">
            <button class="ms-btn arrow-btn position-relative border mt-4 me-3">
                <i class="fa-solid fa-arrow-left"></i>
            </button>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
            <button class="ms-btn arrow-btn position-relative border mt-4">
                <i class="fa-solid fa-arrow-right"></i>
            </button>
        </div>
        </div>
        <img class="ms-bg left" src="../assets/img/shape.png" alt="rounded-bg">
        <img class="ms-bg right" src="../assets/img/shape2.png" alt="rounded-bg-2">
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

.ms-margin {
    margin-top: 107px;
}

h4 {
    color: $brand-primary;
}

.ms-card {
    width: 30%;
    margin: 6rem 1rem 0 0;
    border-radius: 20px;
    border: none;
    background-color: #fef5f0;

    img {
        max-width: 50%;
        margin: -60px auto 0 auto;
    }
}

.card-social {
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

.ms-bg {
    position: absolute;
    z-index: -1;

    &.left {
        top: 80px;
        left: 0;
    }

    &.right {
        top: 0;
        right: 0;
    }
}

.ms-btn-ctn {
    color: gray;
    
    .fa-circle {
        font-size: 0.6rem;
        margin-right: 1rem;
        cursor: pointer;

        &:hover {
            color: black;
            transform: scale(1.2);
            transition: 0.2s;
        }
    }


}


</style>