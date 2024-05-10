<template>
    <div>
        <NavbarStyleTwo />
        <MainBanner />
        <AboutUsStyleTwo />
        <!-- <ServicesContant /> -->
        <CheckOurServices />
        <!-- <WhatWeDo /> -->
        <WhatOurClientsSaying />
        <OurSomeRecentWorks />
        <!-- <Partner /> -->
        <OurTeamStyleTwo />
        <StartYourProjectWithUs />
        <LatestBlog />
        <Footer />
    </div>
</template>

<script>
    import NavbarStyleTwo from '../layouts/Navbar'
    import MainBanner from '../components/HomeTwo/MainBanner'
    import ServicesContant from '../components/HomeTwo/ServicesContant'
    import AboutUsStyleTwo from '../components/Common/AboutUsStyleTwo'
    import CheckOurServices from '../components/Common/CheckOurServices'
    // import WhatWeDo from '../components/Common/WhatWeDo'
    import WhatOurClientsSaying from '../components/Common/WhatOurClientsSaying'
    import OurSomeRecentWorks from '../components/Common/OurSomeRecentWorks'
    import Partner from '../components/Common/Partner'
    import OurTeamStyleTwo from '../components/Common/OurTeamStyleTwo'
    import StartYourProjectWithUs from '../components/Common/StartYourProjectWithUs'
    import LatestBlog from '../components/Common/LatestBlog'
    import Footer from '../layouts/Footer'
    import axios from 'axios';


    export default {
        components: {
            NavbarStyleTwo,
            MainBanner,
            ServicesContant,
            AboutUsStyleTwo,
            CheckOurServices,
            // WhatWeDo,
            WhatOurClientsSaying,
            OurSomeRecentWorks,
            Partner,
            OurTeamStyleTwo,
            StartYourProjectWithUs,
            LatestBlog,
            Footer,
        },
    data() {
        return {
            seoData: null,
        }
    },
    created: async function () {
        const { slug } = this.$route.params
        const reaponse = await axios.get(`https://cms.ainflow.co.in/api/pages?filters[slug][$eq]=index&populate=deep,5`, { params: { slug } })
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