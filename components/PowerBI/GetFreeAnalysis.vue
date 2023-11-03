<template>
    <div class="seo-analysis-area bg-color ptb-100">
        <div class="container">
            <div class="overview-box">
                <div class="overview-content">
                    <div class="content">
                        <span class="sub-title">AInFlow</span>
                        <h2>Why Power BI?</h2>
                        <p>Power BI is recognized for its user-friendly interface, robust functionality, and seamless
                            integration with other Microsoft products. It has become a leading choice for businesses seeking
                            to harness the power of their data to make better decisions and achieve their goals.</p>
                        <p>Whether you're interested in creating informative reports, tracking performance metrics, or
                            diving into complex data analysis, Power BI has the tools and capabilities you need to succeed.
                        </p>
                        <p>Explore our website for tutorials, case studies, and in-depth guides to unlock the full potential
                            of Power BI for your organization. </p>
                    </div>
                </div>

                <div class="overview-image">
                    <div class="image">
                        <img src="~/assets/images/power-bi/WhyPowerBI.png" alt="image">
                    </div>
                </div>
            </div>
            <div class="row align-items-center">
                <div class="col-lg-6 col-md-12">
                    <div class="analysis-img">
                        <img src="~/assets/images/power-bi/GettingStarted.png" alt="image">
                    </div>
                </div>

                <div class="col-lg-6 col-md-12">

                    <div class="analysis-form">
                        <span class="sub-title">Analysis</span>
                        <h2>Getting Started with Power BI</h2>
                        <p>If you're new to Power BI, getting started is easy. You can download Power BI Desktop, which is a
                            free application for creating reports and visuals. There's also Power BI Service, a cloud-based
                            platform for sharing and collaborating on reports. Additionally, Microsoft offers extensive
                            training resources and a community of users to support your journey.</p>
                        <form>
                            <div class="row">
                                <div class="col-lg-6 col-md-6">
                                    <div class="form-group">
                                        <input type="text" class="form-control" id="your_name" placeholder="Name" required>
                                    </div>
                                </div>

                                <div class="col-lg-6 col-md-6">
                                    <div class="form-group">
                                        <input type="email" class="form-control" id="your_email" placeholder="Email"
                                            required>
                                    </div>
                                </div>

                                <div class="col-lg-6 col-md-6">
                                    <div class="form-group">
                                        <input type="number" class="form-control" id="your_name" placeholder="Phone Number"
                                            required>
                                    </div>
                                </div>

                                <div class="col-lg-6 col-md-6">
                                    <div class="form-group">
                                        <input type="text" class="form-control" id="website" placeholder="Website" required>
                                    </div>
                                </div>
                            </div>
                            <button type="submit" class="default-btn">Check Now</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
</div></template>

<script>

export default {
    name: 'GetFreeAnalysis'
}
</script>