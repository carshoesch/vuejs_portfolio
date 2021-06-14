<template>
  <div class="row text-center">
    <div class="col-md-4">
        <h3 class="sprachen">
            Sprachen
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
                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.sprachen {
    width: 94vw;
    margin: 0 auto;
    border: 1px solid blue;
    padding-bottom: 1.5rem;


}

.skills {

    /* border: 1px solid blue; */
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
    gap: 2rem;
    width: 90vw;
    margin: 0 auto;
    line-height: 2.5rem;

    .ueberMich {
        border: 1px solid black;
        width: 100%;

        img {
            border: 1px solid red;
        }
    }
}
</style>>