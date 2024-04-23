<script>

import FirstSection from './FirstSection.vue';
import QuickSection from './QuickSection.vue';
import OurWorksSection from './OurWorksSection.vue';
import OurProcessSection from './OurProcessSection.vue';
import TeamSection from './TeamSection.vue';
import WhySection from './WhySection.vue';
import SubmitSection from './SubmitSection.vue';

export default {
    name: 'PageMain',
    components: {
        FirstSection,
        QuickSection,
        OurWorksSection,
        OurProcessSection,
        TeamSection,
        WhySection,
        SubmitSection
    }
}

</script>

<template>

    <main>
        <FirstSection></FirstSection>
        <QuickSection></QuickSection>
        <OurWorksSection></OurWorksSection>
        <OurProcessSection></OurProcessSection>
        <TeamSection></TeamSection>
        <WhySection></WhySection>
        <SubmitSection></SubmitSection>
    </main>

</template>

<style scoped lang="scss"></style>
