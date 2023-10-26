<template>
    <div class="seo-analysis-area bg-color ptb-100">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6 col-md-12">
                    <div class="analysis-img">
                        <img src="~/assets/images/seo-analysis.png" alt="Image">
                    </div>
                </div>

                <div class="col-lg-6 col-md-12">
                    <div class="analysis-form">
                        <span class="sub-title">Analysis</span>
                        <h2>Stay Informed, Stay Safe</h2>
                        <p>In a constantly evolving digital landscape, staying informed and proactive is your best defense. End user protection is not just a choice; it's a responsibility. By adopting the right strategies and tools, you can confidently navigate the digital world while protecting your digital identity and assets.</p>
                        <p>Join us in the journey to safeguard your digital world. Explore our resources, ask questions, and share your insights to empower yourself and others in the realm of end user protection. </p>
                        <form>
                            <div class="row">
                                <div class="col-lg-6 col-md-6">
                                    <div class="form-group">
                                        <input type="text" class="form-control" id="your_name" placeholder="Name" required>
                                    </div>
                                </div>

                                <div class="col-lg-6 col-md-6">
                                    <div class="form-group">
                                        <input type="email" class="form-control" id="your_email" placeholder="Email" required>
                                    </div>
                                </div>

                                <div class="col-lg-6 col-md-6">
                                    <div class="form-group">
                                        <input type="number" class="form-control" id="your_name" placeholder="Phone Number" required>
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
    </div>
</template>

<script>

export default {
    name: 'GetFreeAnalysis'
}
</script>