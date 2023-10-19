<template>
    <div>
        <NavbarStyleFour />
        <PageTitle pageTitle="VAPT" />
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
    import CreativeSolutions from '../components/VAPT/CreativeSolutions'
    import CoreBusiness from '../components/VAPT/CoreBusiness'
    import GetFreeAnalysis from '../components/VAPT/GetFreeAnalysis'
    import StartYourProjectWithUs from '../components/Common/StartYourProjectWithUs'
    import Footer from '../layouts/Footer'
    import axios from 'axios';

    export default {
        components: {
            NavbarStyleFour,
            PageTitle,
            CreativeSolutions,
            CoreBusiness,
            GetFreeAnalysis,
            StartYourProjectWithUs,
            Footer,
        },
    data() {
        return {
            seoData: null,
        }
    },
    created: async function () {
        const { slug } = this.$route.params
        const reaponse = await axios.get(`https://cms.ainflow.co.in/api/pages?filters[slug][$eq]=vapt&populate=deep,5`, { params: { slug } })
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