<template>
 <section class="page-section" id="skills">
              <div class="container">
                  <div class="text-center">
                      <h2 class="section-heading text-uppercase">Über mich</h2>
                      <h3 class="section-subheading text-muted">Sportbegeistert, Sweet-Gourmet und Rätsel-Enthusiast. 
                          Doch vor allem bin ich Software-Entwickler mit einer Leidenschaft für die Erstellung intuitiver, benutzerfreundlicher Web-Erlebnisse. Erst gemeinsam werden gute Projekte großartig.</h3>
                  </div>
  <div class="row text-center">
    <div class="col-md-4">
        <h3 class="sprachen">
            Sprachen/Skills
        </h3>
        <div class="skills">
            <div class="my-3 skill" v-for="(skill, index) in MySkills" :key="index">
                <i :class="skill.image"></i>
                <br>
                {{ skill.language }}
            </div>
        </div>
    </div>
</div>
 </div>
          </section>
</template>

<script>
export default {
    name: "UeberMich",
    data() {
        return {
            MySkills: [
                {
                    language: "HTML", 
                    image: 'fab fa-html5 fa-4x'
                },
                {
                    language: "CSS", 
                    image: 'fab fa-css3 fa-4x'
                },
                {
                    language: "JavaScript", 
                    image: 'fab fa-js-square fa-4x'
                },
                {
                    language: "VueJS", 
                    image: 'fab fa-vuejs fa-4x'
                },
                {
                    language: "MSSQL", 
                    image: 'fas fa-database fa-4x'
                },
                {
                    language: "Python", 
                    image: 'fab fa-python fa-4x'
                },
                {
                    language: "Git",
                    image: 'fab fa-git fa-4x'
                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.col-md-4{

/*     border: 1px solid red;
 */    width: 100%;

    .sprachen {
        width: 90%;
        margin: 0 auto;
        padding-bottom: 1.5rem;

    }

    .skills {

        /* border: 1px solid blue; */
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        gap: 2rem;
        width:90%;
        margin: 0 auto;
        line-height: 2.5rem;

    }
}
</style>>