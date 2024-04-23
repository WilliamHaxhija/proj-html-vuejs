<script>
    
    //*****COMPONENTS*****

    import PageHeader from './components/PageHeader.vue';
    import PageMain from './components/PageMain.vue';
    import PageFooter from './components/PageFooter.vue';

    export default {
      components: {
        PageHeader,
        PageMain,
        PageFooter
      },

        //*****DATA*****

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
				logo: 'logo.png',
                footerLinks: [
                    'About Us',
                    'Portfolio',
                    'Pricing',
                    'Career',
                    'Contact'
                ]
            }
        }
    }

</script>

<template>

    <!-- HEADER -->
    <PageHeader :logoImg="logo" :navLinks="navBar"></PageHeader>

    <!-- MAIN -->
    <PageMain></PageMain>
    
    <!-- FOOTER -->
    <PageFooter :logoImg="logo" :links="footerLinks"></PageFooter>

</template>

<style lang="scss">

@use './style/generic.scss';

</style>
