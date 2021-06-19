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
          <!-- Portfolio Modals-->
          <!-- Portfolio item 1 modal popup-->
          <div class="portfolio-modal modal fade" id="portfolioModal1" tabindex="-1" role="dialog" aria-hidden="true">
              <div class="modal-dialog">
                  <div class="modal-content">
                      <div class="close-modal" data-bs-dismiss="modal"><img src="assets/img/close-icon.svg" alt="Close modal" /></div>
                      <div class="container">
                          <div class="row justify-content-center">
                              <div class="col-lg-8">
                                  <div class="modal-body">
                                      <!-- Project details-->
                                      <h2 class="text-uppercase">Project Name</h2>
                                      <p class="item-intro text-muted">Lorem ipsum dolor sit amet consectetur.</p>
                                      <img class="img-fluid d-block mx-auto" src="assets/img/portfolio/1.jpg" alt="..." />
                                      <p>Use this area to describe your project. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est blanditiis dolorem culpa incidunt minus dignissimos deserunt repellat aperiam quasi sunt officia expedita beatae cupiditate, maiores repudiandae, nostrum, reiciendis facere nemo!</p>
                                      <ul class="list-inline">
                                          <li>
                                              <strong>Client:</strong>
                                              Threads
                                          </li>
                                          <li>
                                              <strong>Category:</strong>
                                              Illustration
                                          </li>
                                      </ul>
                                      <button class="btn btn-primary btn-xl text-uppercase" data-bs-dismiss="modal" type="button">
                                          <i class="fas fa-times me-1"></i>
                                          Close Project
                                      </button>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- Portfolio item 2 modal popup-->
          <div class="portfolio-modal modal fade" id="portfolioModal2" tabindex="-1" role="dialog" aria-hidden="true">
              <div class="modal-dialog">
                  <div class="modal-content">
                      <div class="close-modal" data-bs-dismiss="modal"><img src="assets/img/close-icon.svg" alt="Close modal" /></div>
                      <div class="container">
                          <div class="row justify-content-center">
                              <div class="col-lg-8">
                                  <div class="modal-body">
                                      <!-- Project details-->
                                      <h2 class="text-uppercase">Project Name</h2>
                                      <p class="item-intro text-muted">Lorem ipsum dolor sit amet consectetur.</p>
                                      <img class="img-fluid d-block mx-auto" src="assets/img/portfolio/2.jpg" alt="..." />
                                      <p>Use this area to describe your project. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est blanditiis dolorem culpa incidunt minus dignissimos deserunt repellat aperiam quasi sunt officia expedita beatae cupiditate, maiores repudiandae, nostrum, reiciendis facere nemo!</p>
                                      <ul class="list-inline">
                                          <li>
                                              <strong>Client:</strong>
                                              Explore
                                          </li>
                                          <li>
                                              <strong>Category:</strong>
                                              Graphic Design
                                          </li>
                                      </ul>
                                      <button class="btn btn-primary btn-xl text-uppercase" data-bs-dismiss="modal" type="button">
                                          <i class="fas fa-times me-1"></i>
                                          Close Project
                                      </button>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- Portfolio item 3 modal popup-->
          <div class="portfolio-modal modal fade" id="portfolioModal3" tabindex="-1" role="dialog" aria-hidden="true">
              <div class="modal-dialog">
                  <div class="modal-content">
                      <div class="close-modal" data-bs-dismiss="modal"><img src="assets/img/close-icon.svg" alt="Close modal" /></div>
                      <div class="container">
                          <div class="row justify-content-center">
                              <div class="col-lg-8">
                                  <div class="modal-body">
                                      <!-- Project details-->
                                      <h2 class="text-uppercase">Project Name</h2>
                                      <p class="item-intro text-muted">Lorem ipsum dolor sit amet consectetur.</p>
                                      <img class="img-fluid d-block mx-auto" src="assets/img/portfolio/3.jpg" alt="..." />
                                      <p>Use this area to describe your project. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est blanditiis dolorem culpa incidunt minus dignissimos deserunt repellat aperiam quasi sunt officia expedita beatae cupiditate, maiores repudiandae, nostrum, reiciendis facere nemo!</p>
                                      <ul class="list-inline">
                                          <li>
                                              <strong>Client:</strong>
                                              Finish
                                          </li>
                                          <li>
                                              <strong>Category:</strong>
                                              Identity
                                          </li>
                                      </ul>
                                      <button class="btn btn-primary btn-xl text-uppercase" data-bs-dismiss="modal" type="button">
                                          <i class="fas fa-times me-1"></i>
                                          Close Project
                                      </button>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- Portfolio item 4 modal popup-->
          <div class="portfolio-modal modal fade" id="portfolioModal4" tabindex="-1" role="dialog" aria-hidden="true">
              <div class="modal-dialog">
                  <div class="modal-content">
                      <div class="close-modal" data-bs-dismiss="modal"><img src="assets/img/close-icon.svg" alt="Close modal" /></div>
                      <div class="container">
                          <div class="row justify-content-center">
                              <div class="col-lg-8">
                                  <div class="modal-body">
                                      <!-- Project details-->
                                      <h2 class="text-uppercase">Project Name</h2>
                                      <p class="item-intro text-muted">Lorem ipsum dolor sit amet consectetur.</p>
                                      <img class="img-fluid d-block mx-auto" src="assets/img/portfolio/4.jpg" alt="..." />
                                      <p>Use this area to describe your project. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est blanditiis dolorem culpa incidunt minus dignissimos deserunt repellat aperiam quasi sunt officia expedita beatae cupiditate, maiores repudiandae, nostrum, reiciendis facere nemo!</p>
                                      <ul class="list-inline">
                                          <li>
                                              <strong>Client:</strong>
                                              Lines
                                          </li>
                                          <li>
                                              <strong>Category:</strong>
                                              Branding
                                          </li>
                                      </ul>
                                      <button class="btn btn-primary btn-xl text-uppercase" data-bs-dismiss="modal" type="button">
                                          <i class="fas fa-times me-1"></i>
                                          Close Project
                                      </button>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- Portfolio item 5 modal popup-->
          <div class="portfolio-modal modal fade" id="portfolioModal5" tabindex="-1" role="dialog" aria-hidden="true">
              <div class="modal-dialog">
                  <div class="modal-content">
                      <div class="close-modal" data-bs-dismiss="modal"><img src="assets/img/close-icon.svg" alt="Close modal" /></div>
                      <div class="container">
                          <div class="row justify-content-center">
                              <div class="col-lg-8">
                                  <div class="modal-body">
                                      <!-- Project details-->
                                      <h2 class="text-uppercase">Project Name</h2>
                                      <p class="item-intro text-muted">Lorem ipsum dolor sit amet consectetur.</p>
                                      <img class="img-fluid d-block mx-auto" src="assets/img/portfolio/5.jpg" alt="..." />
                                      <p>Use this area to describe your project. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est blanditiis dolorem culpa incidunt minus dignissimos deserunt repellat aperiam quasi sunt officia expedita beatae cupiditate, maiores repudiandae, nostrum, reiciendis facere nemo!</p>
                                      <ul class="list-inline">
                                          <li>
                                              <strong>Client:</strong>
                                              Southwest
                                          </li>
                                          <li>
                                              <strong>Category:</strong>
                                              Website Design
                                          </li>
                                      </ul>
                                      <button class="btn btn-primary btn-xl text-uppercase" data-bs-dismiss="modal" type="button">
                                          <i class="fas fa-times me-1"></i>
                                          Close Project
                                      </button>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- Portfolio item 6 modal popup-->
          <div class="portfolio-modal modal fade" id="portfolioModal6" tabindex="-1" role="dialog" aria-hidden="true">
              <div class="modal-dialog">
                  <div class="modal-content">
                      <div class="close-modal" data-bs-dismiss="modal"><img src="assets/img/close-icon.svg" alt="Close modal" /></div>
                      <div class="container">
                          <div class="row justify-content-center">
                              <div class="col-lg-8">
                                  <div class="modal-body">
                                      <!-- Project details-->
                                      <h2 class="text-uppercase">Project Name</h2>
                                      <p class="item-intro text-muted">Lorem ipsum dolor sit amet consectetur.</p>
                                      <img class="img-fluid d-block mx-auto" src="assets/img/portfolio/6.jpg" alt="..." />
                                      <p>Use this area to describe your project. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Est blanditiis dolorem culpa incidunt minus dignissimos deserunt repellat aperiam quasi sunt officia expedita beatae cupiditate, maiores repudiandae, nostrum, reiciendis facere nemo!</p>
                                      <ul class="list-inline">
                                          <li>
                                              <strong>Client:</strong>
                                              Window
                                          </li>
                                          <li>
                                              <strong>Category:</strong>
                                              Photography
                                          </li>
                                      </ul>
                                      <button class="btn btn-primary btn-xl text-uppercase" data-bs-dismiss="modal" type="button">
                                          <i class="fas fa-times me-1"></i>
                                          Close Project
                                      </button>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
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
