<template>
    <div class="boxes-area pb-70">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 col-md-6 col-sm-6">
                    <div class="single-boxes-box">
                        <div class="icon">
                            <img src="~/assets/images/SAPResources.png" alt="image">
                            <div class="circles-box">
                                <div class="circle-one"></div>
                            </div>
                        </div>
                        <h3>
                            <NuxtLink to="/">SAP Resources</NuxtLink>
                        </h3>
                        <p>SAP (Systems, Applications, and Products) is a globally renowned software company that provides a
                            wide range of business solutions designed to streamline operations</p>
                        <NuxtLink to="/#" class="learn-more-btn"><i
                                class="left-icon flaticon-next-button"></i> Learn More <i
                                class="right-icon flaticon-next-button"></i></NuxtLink>
                    </div>
                </div>

                <div class="col-lg-4 col-md-6 col-sm-6">
                    <div class="single-boxes-box">
                        <div class="icon">
                            <img src="~/assets/images/ServerHardening.png" alt="image">
                            <div class="circles-box">
                                <div class="circle-one"></div>
                            </div>
                        </div>
                        <h3>
                            <NuxtLink to="/">Server Hardening</NuxtLink>
                        </h3>
                        <p>Server hardening is a crucial system fortification process designed to fortify a server against a
                            myriad of cyber threats by minimizing its attack surface</p>
                        <NuxtLink to="/#" class="learn-more-btn"><i
                                class="left-icon flaticon-next-button"></i> Learn More <i
                                class="right-icon flaticon-next-button"></i></NuxtLink>
                    </div>
                </div>

                <div class="col-lg-4 col-md-6 col-sm-6 offset-lg-0 offset-md-3 offset-sm-3">
                    <div class="single-boxes-box">
                        <div class="icon">
                            <img src="~/assets/images/SharePointDMS.png" alt="image">
                            <div class="circles-box">
                                <div class="circle-one"></div>
                            </div>
                        </div>
                        <h3>
                            <NuxtLink to="/sharepointdms">SharePoint DMS</NuxtLink>
                        </h3>
                        <p>In the dynamic realm of modern business, the art of efficient document management has assumed
                            paramount importance. As organizations amass colossal reservoirs</p>
                        <NuxtLink to="/sharepointdms" class="learn-more-btn"><i
                                class="left-icon flaticon-next-button"></i> Learn More <i
                                class="right-icon flaticon-next-button"></i></NuxtLink>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'ServicesContant'
}
</script>