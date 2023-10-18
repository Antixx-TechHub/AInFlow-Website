<template>
    <div>
        <NavbarStyleFour />
        <PageTitle pageTitle="Power BI" />
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
    import CreativeSolutions from '../components/PowerBI/CreativeSolutions'
    import CoreBusiness from '../components/PowerBI/CoreBusiness'
    import GetFreeAnalysis from '../components/PowerBI/GetFreeAnalysis'
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