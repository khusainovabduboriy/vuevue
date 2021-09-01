<template>
    
<section class="teachers">
<div class="inner-info container">
<p class="our">OUR TEAM</p>
<h3 class="ourwe">Our top dedicated professionals.</h3>

<div class="treners d-flex flex-wrap justify-content-between">
<div class="trener d-flex flex-column justify-content-end" v-for="(obj, key) in teachJSON" :key="key">
  <p class="name">{{obj.title}} <br> <span class="prof">{{obj.txt}}</span> </p>
</div>
</div>

</div>
</section>



</template>
<script>
export default {
        data: () => (
        {
            teachJSON: [
                {
                img: 'img/group13.png',
                title: 'Duglas Walker',
                txt: 'SHIEF STAFF'
                },
                {
                img: 'img/group13.png',
                title: 'Caroline Harrison',
                txt: 'FOUNDER & NANAGER'
                },
                {
                img: 'img/group13.png',
                title: 'Safia Simpson',
                txt: 'WEB DESIGNER'
                }
            ]
        }
    )
}
</script>
<style scoped>
.teachers{
    background: #F2F9FF;
    padding: 92px 0 117px;
    margin-bottom: 180px;
}
.trener{
    height: 450px;
    width: 32%;
background: #E7E7E7;
}
.name{
    font-family: 'Roboto';
font-style: normal;
font-weight: 500;
font-size: 22px;
line-height: 25px;
text-align: center;
color: #262A4E;
}
.prof{
    font-size: 15px;  
}
@media(max-width:767px){
  .trener{
        width: 48%;
        margin: 5px auto;
    }
        h3, .tit{
        font-size: 26px;
line-height: 30px;
    }
}
  
</style>