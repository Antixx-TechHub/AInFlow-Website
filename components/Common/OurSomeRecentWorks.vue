<template>
    <div class="services-area pt-100 pb-70">
        <div class="container">
            <div class="section-title">
                <span class="sub-title">Case Studies</span>
                <h2>Check of Our Some Recent Works & Case Studies</h2>
                <p class="text-center">Case studies offer detailed insights into real-life situations, showcasing
                    practical solutions and outcomes. They are valuable tools for learning, problem-solving, and
                    decision-making in various fields.</p>
            </div>
        </div>

        <div class="container" v-if="casestudies !== []">
            <div class="portfolio-slides owl-carousel owl-theme">
                <carousel :autoplay="true" :loop="true" :autoplayTimeout="7000" :speed="1000" :paginationEnabled="false"
                    :perPageCustom="[[0, 1], [576, 2], [768, 2], [992, 3], [1200, 4],]" :perPage="1"
                    :navigationEnabled="true" navigationNextLabel="<i class='flaticon-chevron'></i>"
                    navigationPrevLabel="<i class='flaticon-back'></i>">

                    <slide v-for="casestudy in casestudies.slice(
            (currentPage - 1) * perPage,
            currentPage * perPage,
        )" :key="casestudy.id">
                        <div class="single-portfolio-item">
                            <NuxtLink :to="'/case-studies-details/' + casestudy.attributes.slug" class="image d-block">
                                <img :src="casestudy.attributes.image.data.attributes.url" alt="blog">
                            </NuxtLink>

                            <div class="content">
                                <h3>
                                    <NuxtLink :to="'/case-studies-details/' + casestudy.attributes.slug">
                                        {{ casestudy.attributes.title }}
                                    </NuxtLink>
                                </h3>
                                <!-- <NuxtLink to="/portfolio-details" class="link-btn"><i class="flaticon-next-button"></i>
                                </NuxtLink> -->
                            </div>
                        </div>
                    </slide>
                </carousel>
            </div>
        </div>
    </div>
</template>

<script>

import axios from 'axios'

export default {
    name: 'Casestudyhome',
    data() {
        return {
            casestudies: [],
            rows: 0,
            currentPage: 1,
            perPage: 6,
        }
    },
    created: async function () {
        const response = await axios.get('https://cms.ainflow.co.in/api/case-studies?populate=*')
        this.casestudies = response.data.data.sort((b, a) => a.id - b.id);
        this.rows = this.casestudies?.length;
    },
}
</script>