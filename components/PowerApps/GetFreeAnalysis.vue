<template>
    <div class="seo-analysis-area bg-color ptb-100">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6 col-md-12">
                    <div class="analysis-img">
                        <img src="~/assets/images/power-apps/whypowerapp.png" alt="image">
                    </div>
                </div>

                <div class="col-lg-6 col-md-12">
                    <div class="analysis-form">
                        <span class="sub-title">Power Apps</span>
                        <h2>Why Power Apps?</h2>
                        <p>Power Apps is a game-changer for businesses of all sizes. With our support, you can unlock the
                            full potential of custom applications, driving growth, efficiency, and innovation. Say goodbye
                            to off-the-shelf software that doesn't quite fit your needs, and say hello to a new era of
                            business optimization.</p>
                        <p> Whether you're looking to improve internal processes, engage with customers more effectively, or
                            innovate in your industry, Power Apps is the key to achieving your goals. Join us on this
                            journey
                            and experience the transformational power of custom applications.</p>

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
    </div>
</template>

<script>

export default {
    name: 'GetFreeAnalysis'
}
</script>