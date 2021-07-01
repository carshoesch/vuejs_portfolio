<template>
  <nav class="navbar navbar-expand-lg navbar-dark fixed-top" :class="{'navbar-shrink': scrollPosition>1}" id="mainNav">
    <div class="container">
            <a class="navbar-brand" href="#page-top">C<span class="normalLetters">arsten</span> H<span class="normalLetters">öschele</span></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
                Menu
                <i class="fas fa-bars ms-1"></i>
            </button>
            <div class="collapse navbar-collapse" id="navbarResponsive">
                <ul class="navbar-nav text-uppercase ms-auto py-4 py-lg-0">
                    <li class="nav-item" v-for="(link, index) in links" :key="index">
                        <a class="nav-link" :href="link.href">{{ link.name }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav> <!-- Masthead--> 
          <header class="masthead">
              <div class="container">
                  <div class="masthead-heading text-uppercase">Hi, ich bin Carsten</div>
                  <!-- <div class="masthead-heading text-uppercase">Moin, Snow hier</div> -->
                  <div class="masthead-subheading">Software-Entwickler & Data Engineer</div>
                  <a class="btn btn-primary btn-xl text-uppercase" href="#portfolio">Zum Portfolio</a>
              </div>
          </header>
</template>

<script>
export default {
    name: "Navbar",
    data() {
        return {
             scrollPosition: null,
             links: [
                 {
                     name: 'Skills',
                     href: '#skills'
                 },
                 {
                     name: 'Portfolio',
                     href: '#portfolio'
                 },
                 {
                     name: 'Werdegang',
                     href: '#werdegang'
                 },
                 {
                     name: 'Contact',
                     href: '#contact'
                 },
             ]
        }
    },
    methods: {
        updateScroll() {
       this.scrollPosition = window.scrollY
        }
    },
        mounted() {
            window.addEventListener('scroll', this.updateScroll);
        }

}
</script>

<style lang="scss" scoped>
    .change_color {
            background-color: #212529;
            width: 100%;
        }

        .masthead {
            height: 100vh;
        }

    </style>
        
 