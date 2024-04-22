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
                    'Contact'
                ],
				logo: 'logo.png'
            }
        }
    }

</script>

<template>

    <PageHeader :logoImg="logo" :navLinks="navBar"></PageHeader>

</template>

<style lang="scss">

@use './style/generic.scss';

</style>
