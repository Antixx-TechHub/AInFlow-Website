<template>
    <div>
        <NavbarStyleFour />
        <PageTitle pageTitle="Internet" />
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
    import CreativeSolutions from '../components/Internet/CreativeSolutions'
    import CoreBusiness from '../components/Internet/CoreBusiness'
    import GetFreeAnalysis from '../components/Internet/GetFreeAnalysis'
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