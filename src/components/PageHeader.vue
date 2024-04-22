<script>

    import PageHero from './PageHero.vue'

    export default {
        name: 'PageHeader',
        components: {
            PageHero
        }
    }

</script>

<template>

    <header>
        <PageHero></PageHero>
    </header>

</template>

<style scoped lang="scss">
    
    @use '../assets/style/generic.scss';

</style>
