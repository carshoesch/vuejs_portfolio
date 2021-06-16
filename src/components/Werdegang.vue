<template>
  <ul class="timeline">
    <li>
        
        <div class="timeline-panel" v-for="(eve, index) in werdegang" :key="index">
            <!-- <div class="timeline-image"></div> -->
            <img class="rounded-circle img-fluid" src="../assets/img/cropped-bullet-point.png" alt="..." />
            <div class="timeline-heading">
                <h4>{{eve.jahreszahl}}</h4>
                <h4 class="subheading">{{eve.titel}}</h4>
            </div>
            <div class="timeline-body"><p class="text-muted">{{eve.beschreibung}}</p></div>
        </div>
    </li>
</ul>
</template>

<script>

export default {
    name: "Werdegang",
    data() {
        return {
            werdegang: [
                {
                    jahreszahl: '2016 – 2019',
                    titel: 'Hochschule Hannover',
                    beschreibung: 'Abschluss: Bachelor of Science - Wirtschaftsinformatik'
                },
                {
                    jahreszahl: '2018',
                    titel: 'Werkstudent bei Heise Medien, Bereich e-Commerce',
                    beschreibung: 'Unterstützung des hauseigenen Shops im Bereich Online-Verkauf, visueller Darstellung und second level support.'
                },
                {
                    jahreszahl: '2019 - 2021',
                    titel: 'Junior Data Engineer',
                    beschreibung: 'Erstellung von Datenbank Analysen mithilfe von SQL, Erstellung von Python-Pipelines zur Extrahierung, Transformation und Laden von externen Daten. Konzeption und Entwicklung von Dashboards und Automatisierungen.'
                },
                {
                    jahreszahl: '2021 -',
                    titel: 'Software Developer',
                    beschreibung: 'Erstellung von E-Commerce Frontend-Lösungen '
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
    img {
        width: 50px;
        height: auto;
        margin-bottom: 2rem
    }
</style>