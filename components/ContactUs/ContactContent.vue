<template>
    <div class="contact-area pb-100">
        <div class="container">
            <div class="section-title">
                <span class="sub-title">Get in Touch</span>
                <h2>Ready to Get Started?<span class="overlay"></span></h2>
                <p>Your email address will not be published. Required fields are marked *</p>
            </div>

            <div class="row">
                <div class="col-lg-6 col-md-12">
                    <div class="contact-image" data-tilt>
                        <img src="~/assets/images/contact.png" alt="image">
                    </div>
                </div>

                <div class="col-lg-6 col-md-12">
                    <div class="contact-form">
                        <form id="contactForm">
                            <form @submit.prevent="submitContent" id="contactForm" action="mailto:rohanshinde9996@gmail.com"
                                method="post" enctype="text/plain">
                                <!-- <form action="rohanshinde9996@gmail.com" method="post" enctype="text/plain"> -->
                                <div class="row">
                                    <div class="col-lg-6 col-md-6">
                                        <div class="form-group">
                                            <input v-model="formData.name" type="text" required name="name" id="name"
                                                class="form-control" placeholder="Your Name">
                                            <div v-if="formErrors.name" class="error-message">{{ formErrors.name }}
                                            </div>
                                        </div>
                                    </div>

                                    <div class="col-lg-6 col-md-6">
                                        <div class="form-group">
                                            <input v-model="formData.email" type="email" required name="email" id="email"
                                                class="form-control" placeholder="Your Email">
                                            <div v-if="formErrors.email" class="error-message">{{ formErrors.email }}
                                            </div>
                                        </div>
                                    </div>

                                    <div class="col-lg-6 col-md-6">
                                        <div class="form-group">
                                            <input v-model="formData.phone_number" type="number" required
                                                name="phone_number" id="phone_number" class="form-control"
                                                placeholder="Your Phone">
                                            <div v-if="formErrors.phone_number" class="error-message">{{
                                                formErrors.phone_number }}</div>
                                        </div>
                                    </div>

                                    <div class="col-lg-6 col-md-6">
                                        <div class="form-group">
                                            <input v-model="formData.msg_subject" type="text" required name="msg_subject"
                                                id="msg_subject" class="form-control" placeholder="Your Subject">
                                            <div v-if="formErrors.msg_subject" class="error-message">{{
                                                formErrors.msg_subject }}</div>
                                        </div>
                                    </div>

                                    <div class="col-lg-12 col-md-12">
                                        <div class="form-group">
                                            <textarea v-model="formData.message" required class="form-control" id="message"
                                                cols="30" rows="6" placeholder="Your Message"></textarea>
                                            <div v-if="formErrors.message" class="error-message">{{ formErrors.message
                                            }}</div>
                                        </div>
                                    </div>

                                    <div class="col-lg-12 col-md-12">
                                        <div class="form-group">
                                            <button type="submit" class="default-btn"><i class='bx bxs-paper-plane'></i>Send
                                                Message<span>
                                                </span> </button>
                                        </div>
                                    </div>
                                </div>
                                <!-- </form> -->
                            </form>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Swal from 'sweetalert2';

export default {
    name: 'Contactme',
    data() {
        return {
            formData: {
                name: '',
                email: '',
                phone_number: '',
                msg_subject: '',
                message: '',
            },
            formErrors: {
                name: '',
                email: '',
                phone_number: '',
                msg_subject: '',
                message: '',
            },
        };
    },
    methods: {
        submitContent() {
            // Clear previous error messages
            this.formErrors = {};

            // Validate form fields
            if (this.formData.name === '') {
                this.formErrors.name = 'Please enter your name';
            }
            if (this.formData.email === '') {
                this.formErrors.email = 'Please enter your email';
            } else if (!this.isValidEmail(this.formData.email)) {
                this.formErrors.email = 'Please enter a valid email address';
            }
            if (this.formData.phone_number === '') {
                this.formErrors.phone_number = 'Please enter your phone number';
            }
            if (this.formData.msg_subject === '') {
                this.formErrors.msg_subject = 'Please enter the subject';
            }
            if (this.formData.message === '') {
                this.formErrors.message = 'Please enter your message';
            }

            // Check if the form is valid
            if (Object.values(this.formErrors).every((error) => error === '')) {
                this.alertContent();
            }
        },
        isValidEmail(email) {
            // Simple email validation using a regular expression
            const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return emailPattern.test(email);
        },
        alertContent() {
            Swal.fire({
                title: 'Great',
                text: 'Thanks for submitting the form',
                icon: 'success',
                timer: 3000,
                timerProgressBar: true,
                showConfirmButton: false,
            });
        },
    },
};
</script>