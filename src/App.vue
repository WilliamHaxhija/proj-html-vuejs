<script>

    import PageHeader from './components/PageHeader.vue';

    export default {
      components: {
        PageHeader
      },
	  data () {
            return {
                navBar: [
                    'Home',
                    'About Us',
                    'Portfolio',
                    'Our Process',
                    'Pricing',
                    'Blog',
                    'Contact',
                    'Get a Quote'
                ]
            }
        }
    }

</script>

<template>

    <PageHeader></PageHeader>

</template>

<style lang="scss">

</style>
