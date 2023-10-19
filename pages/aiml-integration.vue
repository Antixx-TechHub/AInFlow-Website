<template>
    <div>
        <NavbarStyleFour />
        <PageTitle pageTitle="AI-ML Integration" />
        <CreativeSolutions />
        <CoreBusiness />
        <WhyChooseUsAIML />
        <GetFreeAnalysis />
        <!-- <StartYourProjectWithUs /> -->
        <Footer />
    </div>
</template>

<script>
    import NavbarStyleFour from '../layouts/Navbar'
    import PageTitle from '../components/Common/PageTitle'
    import CreativeSolutions from '../components/AIMLIntegration/CreativeSolutions'
    import CoreBusiness from '../components/AIMLIntegration/CoreBusiness'
    import GetFreeAnalysis from '../components/AIMLIntegration/GetFreeAnalysis'
    import WhyChooseUsAIML from '../components/AIMLIntegration/WhyChooseUsAIML'
    // import StartYourProjectWithUs from '../components/Common/StartYourProjectWithUs'
    import Footer from '../layouts/Footer'

    export default {
        components: {
            NavbarStyleFour,
            PageTitle,
            CreativeSolutions,
            CoreBusiness,
            GetFreeAnalysis,
            WhyChooseUsAIML,
            // StartYourProjectWithUs,
            Footer,
        }
    }
</script>