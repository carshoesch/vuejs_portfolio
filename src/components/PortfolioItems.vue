<template>
    <div class="row">
        <div class="col-lg-4 col-sm-6 mb-4 skurr" v-for="(obj, index) in portfolioProject" :key="index">
                <!-- Portfolio item 3-->
                <div class="portfolio-item">
                    <a class="portfolio-link" data-bs-toggle="modal" href="#portfolioModal3">
                        <div class="portfolio-hover">
                            <div class="portfolio-hover-content"><i class="fas fa-plus fa-3x"></i></div>
                        </div>
                        <img class="img-fluid" :src="obj.image" alt="..." />
                    </a>
                    <div class="portfolio-caption">
                        <div class="portfolio-caption-heading">{{ obj.caption }}</div>
                        <br>
                        <button><a :href="obj.link_git" target="_blank">Git-Repo</a></button> &nbsp
                        <button><a :href="obj.link_live" target="_blank">Live-Demo</a></button>
                    </div>
                </div>
            </div>
    </div>
</template>

<script>
export default {
    name: "PortfolioItems",
    data() {
        return {
            portfolioProject: [
                {
                    image: '../assets/img/clipboard_landingpage.png',
                    caption: 'Clipboard Landingpage',
                    link_git: 'https://github.com/carshoesch/clipboard_landing_page',
                    link_live: 'https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.dotcom-monitor.com%2Fblog%2Fde%2F2020%2F05%2F25%2Fmonitoring-applications-written-in-vue-js%2F&psig=AOvVaw2XW5RHczMPIrmJzJO-QPWv&ust=1623838339310000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCKjagq2zmfECFQAAAAAdAAAAABAD'
                },
                {
                    image: '../assets/img/vfr_planner.png',
                    caption: 'Terminkalender eines Rugbyvereins',
                    link_git: 'https://github.com/carshoesch/vfr_planner_vue_firebase'
                },
                {
                    image: '../assets/img/huddle_landingpage.png',
                    caption: 'Huddle Landingpage',
                    link_git: 'https://github.com/carshoesch/huddle'
                },
                {
                    image: '../assets/img/portfolio_v1.png',
                    caption: 'Erstes Portfolio',
                    link_git: 'https://github.com/carshoesch/portfolio_v1'
                },
                {
                    image: '..some/thing/item.png',
                    caption: 'Twotter Blogging',
                    link_git: 'https://github.com/carshoesch/twotter'
                },
                {
                    image: '..some/thing/item.png',
                    caption: 'Vue Todo List',
                    link_git: 'https://github.com/carshoesch/vuejs_todoList'
                },
            ]
        }

    }
}
</script>

<style lang="scss" scoped>

</style>