<template>
  <div class="section" :style="fillstyle">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path :fill="fillvalue" fill-opacity="1" d="M0,160L48,133.3C96,107,192,53,288,42.7C384,32,480,64,576,101.3C672,139,768,181,864,181.3C960,181,1056,139,1152,106.7C1248,75,1344,53,1392,42.7L1440,32L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"></path></svg>
                <div class="section-details flex items-end" :style="{ 'background': 'transparent url(' +  insideimage + ') center 0% no-repeat padding-box;' }">
                    <circle><span class="section-number col-span-1">{{Section.id}}.</span></circle>
                    <span class="section-text col-span-2">{{Section.text}}</span>
                </div>
    </div>
</template>

<script>
export default {
    props: ["Section"],
    data(){
        return{
            styleodd: "background: transparent linear-gradient(134deg, #E6FFFA 0%, #EBF4FF 100%) 0% 0% no-repeat padding-box;"
        }
    },
    computed: {
        insideimage: function(){
            return require("@/static/svg/" + this.Section.image)
        },
        fillvalue: function(){
            if (this.Section.id == 1) return "#FFF";
            return (this.Section.id % 2 == 0) ?  '#FFF' : "#EBF4FF"
        },
        fillstyle: function(){
            return (this.Section.id % 2 == 0) ? this.styleodd  : " "
        }
    }
}
</script>

<style>

</style>