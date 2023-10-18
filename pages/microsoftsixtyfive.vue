<template>
    <div>
        <NavbarStyleFour />
        <PageTitle pageTitle="Microsoft 365" />
        <CreativeSolutions />
        <CoreBusiness />
        <GetFreeAnalysis />
        <StartYourProjectWithUs />
        <Footer />
    </div>
</template>

<script>
    import NavbarStyleFour from '../layouts/Navbar'
    import PageTitle from '../components/Common/PageTitle'
    import CreativeSolutions from '../components/MicrosoftSixtyFive/CreativeSolutions'
    import CoreBusiness from '../components/MicrosoftSixtyFive/CoreBusiness'
    import GetFreeAnalysis from '../components/MicrosoftSixtyFive/GetFreeAnalysis'
    import StartYourProjectWithUs from '../components/Common/StartYourProjectWithUs'
    import Footer from '../layouts/Footer'

    export default {
        components: {
            NavbarStyleFour,
            PageTitle,
            CreativeSolutions,
            CoreBusiness,
            GetFreeAnalysis,
            StartYourProjectWithUs,
            Footer,
        }
    }
</script>