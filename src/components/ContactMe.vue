<template>
  <section
    id="contact"
    class="paralax-mf footer-paralax bg-image sect-mt4 route"
    style="background-image: url(assets/img/overlay-bg.jpg)"
  >
    <div class="overlay-mf"></div>
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="contact-mf">
            <div id="contact" class="box-shadow-full">
              <div class="row">
                <div class="col-md-6">
                  <div class="title-box-2">
                    <h5 class="title-left" data-aos="fade-up">Send Message</h5>
                  </div>
                  <div data-aos="zoom-in">
                    <form action="" class="php-email-form">
                      <div class="row">
                        <div class="col-md-12 mb-3" >
                          <div class="form-group" >
                            <input
                              type="text"
                              name="name"
                              title="Name text"
                              v-model="nameForm"
                              class="form-control"
                              id="name"
                              placeholder="Your Name"
                              required
                            />
                          </div>
                        </div>
                        <div class="col-md-12 mb-3">
                          <div class="form-group">
                            <input
                              type="text"
                              class="form-control"
                              title="Subject text"
                              v-model="subjectForm"
                              name="subject"
                              id="subject"
                              placeholder="Subject"
                              required
                            />
                          </div>
                        </div>
                        <div class="col-md-12">
                          <div class="form-group">
                            <textarea
                              class="form-control textareaForm"
                              title="Message text area"
                              v-model="messageForm"
                              name="message"
                              rows="5"
                              placeholder="Message"
                              required
                            ></textarea>
                          </div>
                        </div>
                        <div class="col-md-12 text-center my-3">
                          <div class="loading">Loading</div>
                          <div class="error-message"></div>
                          <div class="sent-message">
                            Your message has been sent. Thank you!
                          </div>
                        </div>
                        <div class="col-md-12 text-center">
                          <button
                            type="submit"
                            class="button button-a button-big button-rouded"
                            title="Button send message"
                            @click="sendMail"
                          >
                            Send Message
                          </button>
                        </div>
                      </div>
                    </form>
                  </div>
                </div>
                <div class="col-md-6">
                  <div class="title-box-2 pt-4 pt-md-0">
                    <h5 class="title-left" data-aos="fade-up">Get in Touch</h5>
                  </div>
                  <div class="more-info" data-aos="zoom-in">
                    <p class="lead">
                      In case you require of additional information, please do
                      not hesitate to contact me at my email!
                    </p>
                    <ul class="list-ico">
                      <li>
                        <i class="fa-solid fa-location-dot"  title="icon location"></i> Barcelona
                      </li>
                      <li>
                        <i class="fa-solid fa-envelope" title="icon mail"></i>
                        devinschlippe@gmail.com
                      </li>
                    </ul>
                  </div>
                  <div class="socials" data-aos="zoom-in">
                    <ul>
                      <li>
                        <a href="https://github.com/DevinSJ" title="Link to GitHub"
                          ><span class="ico-circle"
                            ><i class="fa-brands fa-github"></i></span
                        ></a>
                      </li>
                      <li>
                        <a
                          href="https://www.linkedin.com/in/devinschlippejusticia"
                          title="Link to LinkedIn"
                          ><span class="ico-circle"
                            ><i class="fa-brands fa-linkedin"></i></span
                        ></a>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactMeComponent",
  data() {
    return {
      nameForm: "",
      subjectForm: "",
      messageForm: "",
    };
  },
  methods: {
    sendMail() {
      window.location.href =
        "mailto:dschlippej81@cepnet.net?subject=" +
        this.subjectForm +
        "&body=" +this.nameForm + '%0D%0A' + 
        this.messageForm;
    },
  },
};
</script>

<style scoped>
.paralax-mf {
  box-shadow: 0 13px 8px -10px rgba(0, 0, 0, 0.1);
  position: relative;
  padding: 8rem 0;
}

.footer-paralax {
  padding: 4rem 0 0 0;
}

.bg-image {
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
  background-position: center center;
}

@media (max-width: 1024px) {
  .bg-image {
    background-attachment: scroll;
  }
}

.sect-mt4 {
  margin-top: 6rem;
}

.overlay-mf {
  background-color: rgba(0, 0, 0, 0.6);
}

.overlay-mf {
  position: absolute;
  top: 0;
  left: 0px;
  padding: 0;
  height: 100%;
  width: 100%;
  opacity: 0.7;
}

.contact-mf {
  margin-top: 4rem;
}

.box-shadow-full {
  padding: 3rem 1.25rem;
  position: relative;
  background-color: #ffffff;
  margin-bottom: 3rem;
  z-index: 2;
  box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.06), 0 2px 5px 0 rgba(0, 0, 0, 0.2);
}

@media (min-width: 768px) {
  .box-shadow-full {
    padding: 3rem;
  }
}

.title-box-2 {
  margin-bottom: 3rem;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.title-left {
  font-size: 2rem;
  position: relative;
}

.title-left:before {
  content: "";
  position: absolute;
  height: 3px;
  background-color: #0078ff;
  width: 100px;
  bottom: -12px;
}

.php-email-form .error-message {
  display: none;
  color: #ffffff;
  background: #ed3c0d;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}

.php-email-form .sent-message {
  display: none;
  color: #fff;
  background: #18d26e;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}

.php-email-form .loading {
  display: none;
  background: #ffffff;
  text-align: center;
  padding: 15px;
}

.php-email-form .loading:before {
  content: "";
  display: inline-block;
  border-radius: 50%;
  width: 24px;
  height: 24px;
  margin: 0 10px -6px 0;
  border: 3px solid #18d26e;
  border-top-color: rgb(255, 255, 255);
  -webkit-animation: animate-loading 1s linear infinite;
  animation: animate-loading 1s linear infinite;
}

.php-email-form input,
.php-email-form textarea {
  border-radius: 0;
  box-shadow: none;
  font-size: 14px;
}

.php-email-form input:focus,
.php-email-form textarea:focus {
  border-color: #0078ff;
}

.php-email-form input {
  padding: 10px 15px;
}

.php-email-form textarea {
  padding: 12px 15px;
  margin-bottom: 0;
}

.php-email-form button[type="submit"] {
  background: #365f91;
  border: 0;
  padding: 10px 24px;
  color: #ffffff;
  transition: 0.4s;
}

.php-email-form button[type="submit"]:hover {
  background: #365f91;
  transform: scale(1.1);
}

@-webkit-keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

@keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

.button {
  display: inline-block;
  padding: 0.3rem 0.6rem;
  text-align: center;
  vertical-align: middle;
  -webkit-user-select: none;
  -moz-user-select: none;
  user-select: none;
  font-size: 1rem;
  border-radius: 0.3rem;
  border: 1px solid transparent;
  transition: all 500ms ease;
  cursor: pointer;
}

.button:focus {
  outline: 0;
}

.button:hover {
  background-color: #365F91;
  color: #ffffff;
  transition: all 500ms ease;
}

.button-a {
  text-decoration: none;
  background-color: #0078ff;
  color: #ffffff;
  border-color: #ffffff;
}

.button-big {
  padding: 0.9rem 2.3rem;
  font-size: 1.2rem;
}

.button-rouded {
  border-radius: 5rem;
}

.socials {
  padding: 2.5rem 0;
}

.socials ul li {
  display: inline-block;
}

.socials .ico-circle {
  height: 40px;
  width: 40px;
  font-size: 1.2rem;
  border-radius: 50%;
  line-height: 1.6;
  margin: 0 15px 0 0;
  box-shadow: 0 0 0 3px #0078ff;
  transition: all 500ms ease;
}

.socials .ico-circle:hover {
  background-color: #0078ff;
  color: #ffffff;
  box-shadow: 0 0 0 3px #ffffff;
  transition: all 500ms ease;
}

.ico-circle {
  height: 100px;
  width: 100px;
  font-size: 2rem;
  border-radius: 50%;
  line-height: 1.55;
  margin-right: 25px !important;
  text-align: center;
  box-shadow: 0 0 0 10px #0078ff;
  color: black;
  display: block;
}

.list-ico {
  line-height: 2;
  list-style: none;
  padding-left: 0;
  margin-bottom: 0;
}

.list-ico span {
  color: #0078ff;
  margin-right: 10px;
}

.more-info, .socials{
  text-align: start !important;
}

.textAreaForm{
  resize: none;
}
</style>