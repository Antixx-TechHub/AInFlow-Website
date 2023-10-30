<template>
    <div>
        <NavbarStyleFour />
        <PageTitle pageTitle="Bussiness Centre" />
        <CreativeSolutions />
        <CoreBusiness />
        <GetFreeAnalysis />
        <Footer />
    </div>
</template>

<script>
    import NavbarStyleFour from '../layouts/Navbar'
    import PageTitle from '../components/Common/PageTitle'
    import CreativeSolutions from '../components/BussinessCentre/CreativeSolutions'
    import CoreBusiness from '../components/BussinessCentre/CoreBusiness'
    import GetFreeAnalysis from '../components/BussinessCentre/GetFreeAnalysis'
    import Footer from '../layouts/Footer'
    import axios from 'axios';

    export default {
        components: {
            NavbarStyleFour,
            PageTitle,
            CreativeSolutions,
            CoreBusiness,
            GetFreeAnalysis,
            Footer,
        },
    data() {
        return {
            seoData: null,
        }
    },
    created: async function () {
        const { slug } = this.$route.params
        const reaponse = await axios.get(`https://cms.ainflow.co.in/api/pages?filters[slug][$eq]=bussiness-center&populate=deep,5`, { params: { slug } })
        this.details = reaponse.data.data;
        const pageData = this.details.length > 0 ? this.details[0] : {};
        if (pageData?.attributes?.seo) {
            this.seoData = pageData.attributes.seo;
        }
    },
    head({ $seo }) {
        return $seo({
            title: this.seoData?.metaTitle,
            description: this.seoData?.metaDescription,
            keywords: this.seoData?.keywords,
        });
    },
}
</script>