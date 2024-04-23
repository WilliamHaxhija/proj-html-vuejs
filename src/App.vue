<script>

    import PageHeader from './components/PageHeader.vue';
    import FirstSection from './components/FirstSection.vue';
    import QuickSection from './components/QuickSection.vue';
    import OurWorksSection from './components/OurWorksSection.vue';

    export default {
      components: {
        PageHeader,
        FirstSection,
        QuickSection,
        OurWorksSection
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
    <QuickSection></QuickSection>
    <OurWorksSection></OurWorksSection>

</template>

<style lang="scss">

@use './style/generic.scss';

</style>
