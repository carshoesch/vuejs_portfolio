<template>

<section class="page-section bg-light" id="portfolio">
              <div class="container">
                  <div class="text-center">
                      <h2 class="section-heading text-uppercase">Portfolio</h2>
                      <h3 class="section-subheading text-muted">Here you go: Eine kleine Zusammenstellung meiner bisherigen, privat umgesetzten Projekte.</h3>
                  </div>
    <div class="row">
        <div class="col-lg-4 col-sm-6 mb-4 skurr" v-for="(obj, index) in portfolioProject" :key="index">
                <!-- Portfolio item 3-->
                <div class="portfolio-item">
                    <!--<a class="portfolio-link" data-bs-toggle="modal" href="#portfolioModal3">
                         <div class="portfolio-hover">
                            <div class="portfolio-hover-content"><i class="fas fa-plus fa-3x"></i></div>
                        </div> 
                        
                    </a>-->
                    <img class="img-fluid" :src=obj.image alt="..." />
                    <div class="portfolio-caption">
                        <div class="portfolio-caption-heading">{{ obj.caption }}</div>
                        <br>
                        <div class="buttons">
                            <button><a :href="obj.link_git" target="_blank">Git-Repo</a></button>&nbsp
                            <button><a :href="obj.link_live" target="_blank">Live-Demo</a></button>
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
    name: "PortfolioItems",
    data() {
        return {
            portfolioProject: [
                {
                    image: require('../assets/img/weather_app.png'),
                    caption: 'Vue Mobile Weather-App',
                    link_git: 'https://github.com/carshoesch/vuejs_weather-app'
                },
                {
                    image: require('../assets/img/vfr_planner.png'),
                    caption: 'Terminkalender eines Rugbyvereins',
                    link_git: 'https://github.com/carshoesch/vfr_planner_vue_firebase',
                    link_live: 'https://vfr-planner-61ddb.web.app/'
                },
                {
                    image: require('../assets/img/clipboard_landingpage.png'),
                    caption: 'Clipboard Landingpage',
                    link_git: 'https://github.com/carshoesch/clipboard_landing_page',
                    link_live: 'https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.dotcom-monitor.com%2Fblog%2Fde%2F2020%2F05%2F25%2Fmonitoring-applications-written-in-vue-js%2F&psig=AOvVaw2XW5RHczMPIrmJzJO-QPWv&ust=1623838339310000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCKjagq2zmfECFQAAAAAdAAAAABAD'
                },
                {
                    image: require('../assets/img/huddle_landingpage.png'),
                    caption: 'Huddle Landingpage',
                    link_git: 'https://github.com/carshoesch/huddle',
                    link_live: 'https://carshoesch.github.io/huddle/',
                },
                {
                    image: require('../assets/img/portfolio_v1.png'),
                    caption: 'Erstes Portfolio',
                    link_git: 'https://github.com/carshoesch/portfolio_v1',
                    link_live: 'https://carshoesch.github.io/portfolio_v1/',
                },
                {
                    image: require('../assets/img/vue_todoList_omo.png'),
                    caption: 'Vue Todo List',
                    link_git: 'https://github.com/carshoesch/vuejs_todoList'
                },
                {
                    image: require('../assets/img/vue_twotter.png'),
                    caption: 'Twotter Blogging',
                    link_git: 'https://github.com/carshoesch/twotter'
                },
            ]
        }

    }
}
</script>

<style lang="scss" scoped>

    html {
        font-size: 16rem;
    }
    /* 420 width 225 height */
    .portfolio-item {
       /*  display: flex;
        flex-wrap: wrap; */

        img {
            height: 14rem;
            width: 26rem;
        }

        .portfolio-caption {
            display: flex;
            flex-direction: column;
            align-items: center;


            .portfolio-caption-heading {
                height: 5rem;
                max-width: 26rem;
                font-size: 1.3rem;
                padding-bottom: 5rem;

                
            }

            button {
                    border-radius: 5px;
                }

        }
    }

    a {
        text-decoration: none;
    }
</style>