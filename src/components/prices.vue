<template>
    
<section class="mb">

<div class="container">
<div class="priceinfo d-flex justify-content-between align-items-center">
  <div class="txts">
    <p class="ourtxt">OUR PRICING</p>
    <p class="tit">Choose A Plan That’s Right For You</p>
  </div>
  <div class="mover d-flex">
    <p class="date colorchange">Monthly</p>
    <div class="bigger d-flex align-items-center " v-on:click='move'>
      <div class="roll"></div>
    </div> <p class="date">Yearly</p>
  </div>
</div>

<div class="cards d-flex justify-content-between flex-wrap">


  <div class="pricecard pr1 d-flex flex-column align-items-center" v-on:mouseover="globalChange" v-on:mouseleave="globalLeave">
    <p class="name nm1">Basic Plan</p>
    <div class="imgg "><img src="img/group13.png" alt=""></div>  
    <p class="gentit gen1"><span class="dol dol1">$50</span> /Month</p>
    <p class="sectit sec1">Graphic Design <br>
      Web Design <br>
      UI/UX <br>
      HTML/CSS <br> 
      SEO Marketing <br>
      Business Analysis</p>
      <a href="#" class="start st1">Start Now</a>
  </div>
  <div class="pricecard pr2 d-flex flex-column align-items-center" v-on:mouseover="globalChange2" v-on:mouseleave="globalLeave2">
    <p class="name nm2">Standart Plan</p>
    <div class="imgg"><img src="img/group13.png" alt=""></div>  
    <p class="gentit gen2"><span class="dol dol2">$99</span> /Month</p>
    <p class="sectit sec2">Graphic Design <br>
      Web Design <br>
      UI/UX <br>
      HTML/CSS <br> 
      SEO Marketing <br>
      Business Analysis</p>
      <a href="#" class="start st2">Start Now</a>
  </div>
  <div class="pricecard pr3 d-flex flex-column align-items-center" v-on:mouseover="globalChange3" v-on:mouseleave="globalLeave3">
    <p class="name nm3">Premium Plan</p>
    <div class="imgg "><img src="img/group13.png" alt=""></div>  
    <p class="gentit gen3"><span class="dol dol3">$150</span> /Month</p>
    <p class="sectit sec3">Graphic Design <br>
      Web Design <br>
      UI/UX <br>
      HTML/CSS <br> 
      SEO Marketing <br>
      Business Analysis</p>
      <a href="#" class="start st3">Start Now</a>
  </div>
</div>




</div>

</section>

</template>
<script>
import $ from 'jquery'
export default {
    data(){
        return{}
    },
    methods:{
        move: function(){
        $('.roll').toggleClass('move');
        $('.date').toggleClass('colorchange');
        },
        globalChange: function(){
        $('.nm1').addClass('white');
        $('.gen1').addClass('white');
        $('.sec1').addClass('white');
        $('.dol1').addClass('white');
        $('.st1').addClass('changes');
        $('.pr1').addClass('bgblue');
        },
        globalLeave: function(){
        $('.nm1').removeClass('white');
        $('.gen1').removeClass('white');
        $('.sec1').removeClass('white');
        $('.dol1').removeClass('white');
        $('.st1').removeClass('changes');
        $('.pr1').removeClass('bgblue');
        },



          globalChange2: function(){
        $('.nm2').addClass('white');
        $('.gen2').addClass('white');
        $('.sec2').addClass('white');
        $('.dol2').addClass('white');
        $('.st2').addClass('changes');
        $('.pr2').addClass('bgblue');
        },
        globalLeave2: function(){
        $('.nm2').removeClass('white');
        $('.gen2').removeClass('white');
        $('.sec2').removeClass('white');
        $('.dol2').removeClass('white');
        $('.st2').removeClass('changes');
        $('.pr2').removeClass('bgblue');
        },



          globalChange3: function(){
        $('.nm3').addClass('white');
        $('.gen3').addClass('white');
        $('.sec3').addClass('white');
        $('.dol3').addClass('white');
        $('.st3').addClass('changes');
        $('.pr3').addClass('bgblue');
        },
        globalLeave3: function(){
        $('.nm3').removeClass('white');
        $('.gen3').removeClass('white');
        $('.sec3').removeClass('white');
        $('.dol3').removeClass('white');
        $('.st3').removeClass('changes');
        $('.pr3').removeClass('bgblue');
        },
    }
}

</script>
<style scoped>
.bigger{
    width: 52px;
height: 23px;
background: #2370C8;
border-radius: 10px;
box-shadow: 0px 0px 5px 1px rgb(100, 100, 100);
margin: 0 12px;
}
.roll{
    width: 26px;
height: 26px;
background: #FFFFFF;
box-shadow: 0px 1px 7px rgba(0, 0, 0, 0.42);
border-radius: 50%;
transition: all 0.5s;
}
.move{
    transform: translateX(100%);
}
.date{
    font-family: 'Roboto';
font-style: normal;
font-weight: 500;
font-size: 20px;
line-height: 23px;
color: #262A4E;
transition: 0.5s;
}
.colorchange{
    color: #2370C8;
}
.pricecard{
    background: #FFFFFF;
box-shadow: 0px 8px 48px rgba(185, 215, 238, 0.4);
width: 32%;
padding: 45px 0;
transition: 0.5s;
}
.dol{
    font-family: 'Roboto';
font-style: normal;
font-weight: 500;
font-size: 35px;
line-height: 41px;
color: #2370C8;
transition: 0.5s;
}
.start{
    font-family: 'Roboto';
font-style: normal;
font-weight: bold;
font-size: 16px;
line-height: 19px;
color: #FFFFFF;
padding: 11px 36px 12px 28px;
background: #2370C8;
border-radius: 30px;
margin-top: 33px;
transition: 0.5s;
}
.white{
    color: white;
}
.changes{
    color:#2370C8 ;
    background: white;
}
.bgblue{
    background: #2370C8;
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
.ourtxt{
    font-family: 'Roboto';
font-style: normal;
font-weight: 500;
font-size: 20px;
line-height: 30px;
letter-spacing: 0.15em;
color: #2370C8;
}
.tit{
    font-family: 'Roboto';
font-style: normal;
font-weight: 500;
font-size: 48px;
line-height: 56px;
color: #262A4E;
margin-bottom: 20px;
}
.mb{
    
    margin-bottom: 180px;
}
@media (max-width:767px) {
.pricecard{
        width: 48%;
        margin: 5px auto;
    }
    .our, .ourtxt{
        font-size: 18px;
    }
        h3, .tit{
        font-size: 26px;
line-height: 30px;
    }
}
</style>