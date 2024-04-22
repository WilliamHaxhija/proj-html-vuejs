<script>

    import PageHeader from './components/PageHeader.vue';
    import FirstSection from './components/FirstSection.vue';

    export default {
      components: {
        PageHeader,
        FirstSection
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
    <FirstSection></FirstSection>

</template>

<style lang="scss">

@use './style/generic.scss';

</style>
