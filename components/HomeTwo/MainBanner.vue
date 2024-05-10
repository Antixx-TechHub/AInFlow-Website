<template>
    <div>
        <CoolLightBox :items="items" :fullScreen="true" :index="index" @close="index = null">
        </CoolLightBox>

        <div class="home-wrapper-area">
            <div class="container-fluid">
                <div v-if="banner !== null" class="row">
                    <div class="home-slides owl-carousel owl-theme">
                        <carousel :autoplay="true" :loop="true" :autoplayTimeout="7000" :speed="5000" :paginationEnabled="false" :perPageCustom="[[0, 1]]"
                            :perPage="1" :navigationEnabled="true" navigationNextLabel="<i class='flaticon-back'></i>"
                            navigationPrevLabel="<i class='flaticon-chevron'></i>">
                            <slide>
                                <div class="single-banner-item">
                                    <div class="row align-items-center">
                                        <div class="col-lg-6 col-md-12">
                                            <div class="banner-content">
                                                <span class="sub-title">AInFlow</span>
                                                <h3>Where AI Meets Innovation AInFlow
                                                </h3>
                                                <p>Welcome to AInFlow, your gateway to the world of artificial
                                                    intelligence. We are dedicated to harnessing the transformative
                                                    potential of AI to help businesses and individuals thrive in the
                                                    digital age. Our commitment to innovation, customization, and proven
                                                    results sets us apart in the AI landscape.</p>
                                                <div class="btn-box">
                                                    <div class="d-flex align-items-center">
                                                        <NuxtLink to="/contact-us" class="default-btn">Get Started
                                                        </NuxtLink>
                                                        <div class="video-btn popup-youtube"
                                                            v-for="(image, imageIndex) in items" :key="imageIndex"
                                                            @click="index = imageIndex" style="cursor: pointer">
                                                            <i class="flaticon-play-button"></i>
                                                            Watch Video
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>

                                        <div class="col-lg-6 col-md-12">
                                            <div class="banner-image">
                                                <img src="~/assets/images/banner1.png" alt="image">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </slide>

                            <slide>
                                <div class="single-banner-item">
                                    <div class="row align-items-center">
                                        <div class="col-lg-6 col-md-12">
                                            <div class="banner-content">
                                                <span class="sub-title">AInFlow</span>
                                                <h3>Innovating with Intelligence Welcome to AInFlow
                                                </h3>
                                                <p>Welcome to AInFlow, the driving force behind AI-driven innovation. We
                                                    are dedicated to helping businesses, organizations, and individuals
                                                    unlock the immense potential of artificial intelligence. Our
                                                    commitment to delivering intelligent solutions, customized to your
                                                    unique needs, sets us apart.</p>
                                                <div class="btn-box">
                                                    <div class="d-flex align-items-center">
                                                        <NuxtLink to="/contact-us" class="default-btn">Get Started
                                                        </NuxtLink>
                                                        <div class="video-btn popup-youtube"
                                                            v-for="(image, imageIndex) in items" :key="imageIndex"
                                                            @click="index = imageIndex" style="cursor: pointer">
                                                            <i class="flaticon-play-button"></i>
                                                            Watch Video
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>

                                        <div class="col-lg-6 col-md-12">
                                            <div class="banner-image">
                                                <img src="~/assets/images/banner2.png" alt="image">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </slide>

                            <slide>
                                <div class="single-banner-item">
                                    <div class="row align-items-center">
                                        <div class="col-lg-6 col-md-12">
                                            <div class="banner-content">
                                                <span class="sub-title">AInFlow</span>
                                                <h3>AI-Powered Solutions for a Smarter World
                                                </h3>
                                                <p>Welcome to AInFlow, your trusted partner in AI-powered
                                                    transformation. Our passion for AI innovation drives us to deliver
                                                    exceptional solutions that empower your business and elevate your
                                                    potential. We're committed to making artificial intelligence
                                                    accessible and effective for everyone.</p>
                                                <div class="btn-box">
                                                    <div class="d-flex align-items-center">
                                                        <NuxtLink to="/contact-us" class="default-btn">Get Started
                                                        </NuxtLink>
                                                        <div class="video-btn popup-youtube"
                                                            v-for="(image, imageIndex) in items" :key="imageIndex"
                                                            @click="index = imageIndex" style="cursor: pointer">
                                                            <i class="flaticon-play-button"></i>
                                                            Watch Video
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>

                                        <div class="col-lg-6 col-md-12">
                                            <div class="banner-image">
                                                <img src="~/assets/images/banner3.png" alt="image">
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </slide>

                        </carousel>
                    </div>
                </div>
            </div>

            <div class="shape1"><img src="~/assets/images/shape/shape1.png" alt="image"></div>
            <div class="shape2"><img src="~/assets/images/shape/shape2.png" alt="image"></div>
            <div class="shape3"><img src="~/assets/images/shape/shape3.png" alt="image"></div>
            <div class="shape4"><img src="~/assets/images/shape/shape4.png" alt="image"></div>
            <div class="shape5"><img src="~/assets/images/shape/shape5.png" alt="image"></div>
            <div class="shape6"><img src="~/assets/images/shape/shape6.png" alt="image"></div>
            <div class="shape7"><img src="~/assets/images/shape/shape7.png" alt="image"></div>
            <div class="shape8"><img src="~/assets/images/shape/shape8.png" alt="image"></div>
            <div class="shape13"><img src="~/assets/images/shape/shape13.png" alt="image"></div>
            <div class="shape14"><img src="~/assets/images/shape/shape14.png" alt="image"></div>
        </div>
    </div>
</template>

<script>
import CoolLightBox from 'vue-cool-lightbox'
import 'vue-cool-lightbox/dist/vue-cool-lightbox.min.css'
import axios from 'axios'

export default {
    name: 'MainBanner',
    components: { CoolLightBox },
    data() {
        return {
            banner: null,
        }
    },
    created: async function () {
        const response = await axios.get('https://cms.antixxtechhub.in/api/blogs?populate=*')
        const { data: { attributes } } = response.data
        this.banner = attributes
    },
}
</script>