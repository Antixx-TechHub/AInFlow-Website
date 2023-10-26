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
                        <span class="sub-title">EMS</span>
                        <h2>Contact Us</h2>
                        <p>Ready to take your enterprise to the next level? Contact us today to discuss your specific needs and find out how EMS can help you achieve your business objectives.</p>
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