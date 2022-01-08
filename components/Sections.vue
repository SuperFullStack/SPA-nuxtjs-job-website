<template>
  <div class="sections">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#E6FFFA" fill-opacity="1" d="M0,160L48,165.3C96,171,192,181,288,165.3C384,149,480,107,576,85.3C672,64,768,64,864,53.3C960,43,1056,21,1152,21.3C1248,21,1344,43,1392,53.3L1440,64L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"></path></svg>

            <div class="sections-nav"></div>
            <div class="sec-title mx-auto">Drei einfache Schritte zur Vermittlung neuer Mitarbeiter </div>
            <Section v-for="Section in data" :Section="Section" :key="Section.id" />

            
    </div>
</template>

<script>
export default {
    data(){
        return {
            image: require("@/static/svg/profile_data.svg"),
            data: [{'id': 1, 'text': 'Erstellen dein Lebenslauf', 'image': 'profile_data.svg'},
            {'id': 2, 'text': 'Erstellen dein Lebenslauf', 'image': 'task.svg'},
            {'id': 3, 'text': 'Mit nur einem Klick bewerben', 'image': 'personal_file.svg'}
            ],
        }
    }
}
</script>

<style>
circle{
border-radius: 50%;
background: #F7FAFC 0% 0% no-repeat padding-box;
opacity: 0.5;
}
.section-details{
    padding-top: 40px ;
}
.sec-title{
    margin-top: 30px;
    width: 280px;
    height: 50px;
    text-align: center;
    font: 21px/25px Lato;
    letter-spacing: 0px;
    color: #4A5568;
    opacity: 1;
}
.section-number{
    padding-top: 40px;
    text-align: center;
    font: 130px/156px Lato;
    letter-spacing: 0px;
    color: #718096;
    opacity: 1;
    display: inline-block;
}
.section-text{
    /* margin-left: 162px; */
    /* display: inline-block; */
    text-align: left;
    font: 16px/19px Lato;
    letter-spacing: 0.47px;
    color: #718096;
    opacity: 1;
    margin-bottom: 25px;
}
</style>