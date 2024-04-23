<script>

export default {
    name: 'SubmitSection'
}

</script>

<template>

    <section class="position-relative">
        <div class="container text-center">
            <div class="titles w-50 mx-auto">
                <h4>We Create New Worlds!</h4>
                <h1>Want Tips On Your</h1>
                <h1>Storytelling?</h1>
                <div class="mt-3">Join our newsleter for tips on how to elevate your brand through storytelling.</div>
            </div>
            <div class="input-ctn d-flex justify-content-end align-items-center mt-5 mx-auto p-2">
                <input type="mail" placeholder="Enter your email">
                <button class="ms-btn submit-btn">Submit</button>
            </div>
        </div>
        <img class="shape bottom" src="../assets/img/shape-bottom.png" alt="waves-bottom">
        <img class="shape top" src="../assets/img/shape-top.png" alt="waves-top">
    </section>

</template>

<style scoped lang="scss">

@use '../style/partials/variables.scss' as *;

section {
    background-image: url('../assets/img/counter-bg.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    padding: 5rem 0;
    margin: 8rem 0;
}

.titles {
    color: white;
}

h4 {
    color: $brand-secondary;
}

.input-ctn {
    border-radius: 50px;
    background-color: white;
    max-width: 55%;
}

.submit-btn {
    background-color: rgb(231, 231, 231);
    margin-left: 1rem;
    font-weight: 600;
}

input {
    border: none;
    width: 100%;
    border-radius: 40px;
    padding: 0.5rem 1rem;
}

.shape {
    position: absolute;
    max-width: 100%;
    object-fit: contain;

    &.top {
        top: 0;
        left: 0;
    }

    &.bottom {
        bottom: 0;
        left: 0;
    }
}

</style>