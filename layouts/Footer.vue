<template>
    <footer class="footer-area">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 col-md-6 col-sm-6">
                    <div class="single-footer-widget">
                        <NuxtLink to="/" class="logo">
                            <img src="~/assets/images/ainflowlogo.png" alt="logo">
                        </NuxtLink>
                        <p>In this digital age, we are extremely reliant on data – and the amount of data companies are
                            creating is continually increasing.</p>

                        <ul class="social-link">
                            <li><a href="https://www.facebook.com/" class="d-block" target="_blank"><i
                                        class='bx bxl-facebook'></i></a></li>
                            <li><a href="https://twitter.com/" class="d-block" target="_blank"><i
                                        class='bx bxl-twitter'></i></a></li>
                            <li><a href="https://www.instagram.com/" class="d-block" target="_blank"><i
                                        class='bx bxl-instagram'></i></a></li>
                            <li><a href="https://www.linkedin.com/" class="d-block" target="_blank"><i
                                        class='bx bxl-linkedin'></i></a></li>
                        </ul>
                    </div>
                </div>

                <div class="col-lg-2 col-md-6 col-sm-6">
                    <div class="single-footer-widget pl-5">
                        <h3>QuickLinks</h3>

                        <ul class="footer-links-list">
                            <li>
                                <NuxtLink to="/">Home</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/about-us">About Us</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/contact-us">Contact Us</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/security">Security</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/privacy-policy">Privacy Policy</NuxtLink>
                            </li>
                            
                        </ul>
                    </div>
                </div>

                <div class="col-lg-2 col-md-6 col-sm-6">
                    <div class="single-footer-widget pl-2">
                        <h3>Resources</h3>

                        <ul class="footer-links-list">
                            <li>
                                <NuxtLink to="/portfolio">Portfolio</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/blogs">Blog</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/success-stories">Success Story</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/case-studies">Case Study</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/carrers">Carrer</NuxtLink>
                            </li>
                        </ul>
                    </div>
                </div>

                <div class="col-lg-4 col-md-6 col-sm-6">
                    <div class="single-footer-widget">
                        <h3>Address</h3>

                        <ul class="footer-contact-info">
                            <li><i class='bx bx-map'></i>B702, Bhoomi Paradise, Sector 11 Sanpada, Navi Mumbai, 400705.
                            </li>
                            <li><i class='bx bx-envelope'></i><a href="mailto:hello@rivate.com">ainash@ainflow.co.in</a>
                            </li>
                            <li><i class='bx bx-phone-call'></i><a href="tel:+91-99208 28780">+91-99208 28780 </a>, <a
                                    href="tel:+91-93228 34970">+91-93228 34970 </a></li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="footer-bottom-area">
                <div class="row align-items-center">
                    <div class="col-lg-6 col-md-6">
                        <p><i class='bx bx-copyright'></i> <strong>AINFLOW</strong> Copyright 2023 – All Rights Reserved.
                        </p>
                    </div>

                    <div class="col-lg-6 col-md-6">
                        <ul>
                            <li>
                                <NuxtLink to="/privacy-policy">Privacy Policy</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/terms-of-service">Terms & Conditions</NuxtLink>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="shape16"><img src="~/assets/images/more-home/footer/shape.png" alt="image"></div>
    </footer>
</template>

<script>
export default {
    name: 'FooterTwo'
}
</script>