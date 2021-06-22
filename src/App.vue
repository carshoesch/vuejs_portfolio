<template>
            <Navbar/>
          <!-- Masthead--> 
          <header class="masthead">
              <div class="container">
                  <div class="masthead-heading text-uppercase">Hi, ich bin Carsten</div>
                  <!-- <div class="masthead-heading text-uppercase">Moin, Snow hier</div> -->
                  <div class="masthead-subheading">Software-Entwickler & Data Engineer</div>
                  <a class="btn btn-primary btn-xl text-uppercase" href="#portfolio">Zum Portfolio</a>
              </div>
          </header>
          <!-- Über mich -->
          <section class="page-section" id="skills">
              <div class="container">
                  <div class="text-center">
                      <h2 class="section-heading text-uppercase">Über mich</h2>
                      <h3 class="section-subheading text-muted">Sportbegeistert, Sweet-Gourmet und Rätsel-Enthusiast. 
                          Doch vor allem bin ich Software-Entwickler mit einer Leidenschaft für die Erstellung intuitiver, benutzerfreundlicher Web-Erlebnisse. Erst gemeinsam werden gute Projekte großartig.</h3>
                  </div>
                  <!-- über mich section mit den skills -->
                <UeberMich/>
              </div>
          </section>
          <!-- Portfolio Grid-->
          <section class="page-section bg-light" id="portfolio">
              <div class="container">
                  <div class="text-center">
                      <h2 class="section-heading text-uppercase">Portfolio</h2>
                      <h3 class="section-subheading text-muted">Here you go: Eine kleine Zusammenstellung meiner bisherigen, privat umgesetzten Projekte.</h3>
                  </div>
                  <PortfolioItems/>
              </div>
          </section>
          <!-- About-->
          <section class="page-section" id="werdegang">
              <div class="container">
                  <div class="text-center">
                      <h2 class="section-heading text-uppercase">Werdegang</h2>
                      <h3 class="section-subheading text-muted">Von Backend zu Frontend – vom Beruf zur Leidenschaft! 
                          Die Technologielandschaft in der wir uns bewegen ist vielfältig. 
                          Heute entsteht dies und übermorgen das. 
                          Mein Ziel ist es, nicht auf der Stelle zu stehen, zu lernen, um zukunftsfähige Web-Erlebnisse zu gestalten.</h3>
                  </div>
                  <Werdegang/>
              </div>
          </section>
          <!-- Contact-->
          <section class="page-section" id="contact">
              <div class="container">
                  <div class="text-center">
                      <h2 class="section-heading text-uppercase">Kontaktiert mich</h2>
                  </div>
                  <!-- * * * * * * * * * * * * * * *-->
                  <!-- * * SB Forms Contact Form * *-->
                  <!-- * * * * * * * * * * * * * * *-->
                  <!-- This form is pre-integrated with SB Forms.-->
                  <!-- To make this form functional, sign up at-->
                  <!-- https://startbootstrap.com/solution/contact-forms-->
                  <!-- to get an API token!-->
                  <form id="contactForm" data-sb-form-api-token="API_TOKEN">
                      <div class="row align-items-stretch mb-5">
                          <div class="col-md-6">
                              <div class="form-group">
                                  <!-- Name input-->
                                  <input class="form-control" id="name" type="text" placeholder="Your Name *" data-sb-validations="required" />
                                  <div class="invalid-feedback" data-sb-feedback="name:required">A name is required.</div>
                              </div>
                              <div class="form-group">
                                  <!-- Email address input-->
                                  <input class="form-control" id="email" type="email" placeholder="Your Email *" data-sb-validations="required,email" />
                                  <div class="invalid-feedback" data-sb-feedback="email:required">An email is required.</div>
                                  <div class="invalid-feedback" data-sb-feedback="email:email">Email is not valid.</div>
                              </div>
                              <div class="form-group mb-md-0">
                                  <!-- Phone number input-->
                                  <input class="form-control" id="phone" type="tel" placeholder="Your Phone *" data-sb-validations="required" />
                                  <div class="invalid-feedback" data-sb-feedback="phone:required">A phone number is required.</div>
                              </div>
                          </div>
                          <div class="col-md-6">
                              <div class="form-group form-group-textarea mb-md-0">
                                  <!-- Message input-->
                                  <textarea class="form-control" id="message" placeholder="Your Message *" data-sb-validations="required"></textarea>
                                  <div class="invalid-feedback" data-sb-feedback="message:required">A message is required.</div>
                              </div>
                          </div>
                      </div>
                      <!-- Submit success message-->
                      <!---->
                      <!-- This is what your users will see when the form-->
                      <!-- has successfully submitted-->
                      <div class="d-none" id="submitSuccessMessage">
                          <div class="text-center text-white mb-3">
                              <div class="fw-bolder">Form submission successful!</div>
                              To activate this form, sign up at
                              <br />
                              <a href="https://startbootstrap.com/solution/contact-forms">https://startbootstrap.com/solution/contact-forms</a>
                          </div>
                      </div>
                      <!-- Submit error message-->
                      <!---->
                      <!-- This is what your users will see when there is-->
                      <!-- an error submitting the form-->
                      <div class="d-none" id="submitErrorMessage"><div class="text-center text-danger mb-3">Error sending message!</div></div>
                      <!-- Submit Button-->
                      <div class="text-center"><button class="btn btn-primary btn-xl text-uppercase disabled" id="submitButton" type="submit">Send Message</button></div>
                  </form>
              </div>
          </section>
          <!-- Footer-->
          <footer class="footer py-4">
              <div class="container">
                  <div class="row align-items-center">
                      <div class="col-lg-4 text-lg-start">Copyright &copy; Carsten Höschele</div>
                      <div class="col-lg-4 my-3 my-lg-0">
                          <a class="btn btn-dark btn-social mx-2" href="https://www.xing.com/profile/Carsten_Hoeschele2/cv" target="_blank"><i class="fab fa-xing"></i></a>
                          <a class="btn btn-dark btn-social mx-2" href="https://github.com/carshoesch" target="_blank"><i class="fab fa-github"></i></a>
                      </div>
                      <div class="col-lg-4 text-lg-end">
                          <a class="link-dark text-decoration-none me-3" href="#!">Privacy Policy</a>
                          <a class="link-dark text-decoration-none" href="#!">Terms of Use</a>
                      </div>
                  </div>
              </div>
          </footer>
</template>

<script>

import UeberMich from './components/UeberMich.vue'
import PortfolioItems from './components/PortfolioItems.vue'
import Werdegang from './components/Werdegang.vue'
import Navbar from './components/Navbar.vue'


export default {
  name: 'App',
  components: {
    UeberMich,
    PortfolioItems,
    Werdegang,
    Navbar
  }
}
</script>

<style lang="scss" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */

  header {
    height: 100vh;
  }

}
</style>
