<template>
    <div>
        <NavbarStyleFour />
        <PageTitle pageTitle="Sharepoint DMS" />
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
    import CreativeSolutions from '../components/SharePointDMS/CreativeSolutions'
    import CoreBusiness from '../components/SharePointDMS/CoreBusiness'
    import GetFreeAnalysis from '../components/SharePointDMS/GetFreeAnalysis'
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