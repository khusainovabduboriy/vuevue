<template>
  <div id="app">
    <glava />
<background />
<sec />
<about />
<lemon />
<carousel2 /> 
<teacher />
<prices />
<trust />
<padval />
  </div>
</template>

<script>
import glava from "./components/glava.vue"
import background from "./components/background.vue"
import sec from "./components/sec.vue"
import about from "./components/about.vue"
import lemon from "./components/lemon.vue"
import carousel2 from "./components/carousel2.vue"
import teacher from "./components/teacher.vue"
import prices from "./components/prices.vue"
import trust from "./components/trust.vue"
import padval from "./components/padval.vue"
export default {
  components: {
    glava, background, sec, about, lemon, carousel2, teacher, prices, trust, padval
  },
};
</script>

<style>
@font-face {
  font-family: "Roboto";
  src: url(/fonts/roboto.medium.ttf);
}
* {
  margin: 0;
  padding: 0;
}
  .menu_ul.active {
        transform: translateY(-0%);
    }
.burger {
    width: 25px;
    height: 20px;
    cursor: pointer;
    position: absolute;
    z-index: 100000000;
    margin-right: 40px;
    margin-top: 3px;
    right: 0;
}

.burger__line {
    display: block;
    width: 100%;
    height: 3px;
    background: rgb(255, 255, 255);
    left: 0;
    position: absolute;
    transition: 0.3s all linear;
    display:  none;
}

.burger__line_first {
    top: 0;
}

.burger__line_second,
.burger__line_third {
    top: 50%;
    transform: translateY(-50%);
}

.burger__line_fourth {
    bottom: 0;
}

.burger_active .burger__line_first,
.burger_active .burger__line_fourth {
    opacity: 0;
}

.burger_active .burger__line_second {
    transform: translateY(-50%) rotate(45deg);
}

.burger_active .burger__line_third {
    transform: translateY(-50%) rotate(-45deg);
}

@media(max-width:992px){
    .burger__line{
        display: block;
    }
    .menu_ul {
        display: flex;
        align-items: center;
        flex-direction: column;
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        right: 0;
        justify-content: center;
        transition: 1s;
        z-index: 1000000;
        transform: translateY(-100%);
        background: rgba(0, 0, 0, 0.808);
        padding: 0;
        margin: 0;
    }
  .block{
      width: 48%;
      margin: 5px auto;
  }
  .left, .right{
      margin: 15px auto;
  }
}

@media(max-width:767px){
    .infos{
        flex-direction: column;
    }
    .controls{
        margin: auto;
    }
    .h1{
        font-size: 50px;
        line-height: 58px;
        width: 100%;
    }
    .divvi{
        display: none!important;
    }
    input{
        display: none;
    }
    h4{
        font-size: 26px;
        line-height: 30px; 
        margin-bottom: 15px; 
    }
  
    .our, .ourtxt{
        font-size: 18px;
    }
    .inner{
        margin: auto;
    }
    h3, .tit{
        font-size: 26px;
line-height: 30px;
    }
    .blocks{
        margin-top: 20px;
        margin-bottom: 60px;
    }
    .lemon{
        margin-bottom: 60px;
    }
    .teachers{
        margin-bottom: 60px;
    }
    .about{
        margin-bottom: 60px;
    }
    .mb{
        margin-bottom: 60px;
    }

    .clients{
        padding: 30px 0 20px;
    }
            .priceinfo{
                flex-direction: column;
            }
            .txts{

            display: flex;
            flex-direction: column;
            align-items: center;
            }
            .ourlinks{
                width: 48%;
            } 
            .footul, .foot-tit{
                margin: auto;
                margin-top: 10px;
            }           
            .footerinfo{
                        width: 100%;
                    }

        }
@media(max-width:467px){
    .block{
        width: 100%;
        margin: 5px auto;
    }
    .regtangle{
        width: 100%;
            }
            .trener, .pricecard{
                width: 100%;
                margin: 5px auto;
            }
            .cardi{
                width: 100%;
            }
            .client{
                width: 100%;
                margin: 5px auto;
                    }
                    .ourlinks{
                        width: 100%;
                        text-align: center;
                        display: flex;
                        flex-direction: column;
                        justify-content: center;
                    }
                    .learn{
                        padding: 8px 10px;
                        font-size: 15px;
                    }
                    .date{
                        font-size: 15px;
                    }
                    .bigger{
                        width: 46px;
                        height: 18px;
                    }
                    .roll{
                        width: 23px;
                        height: 23px;
                    }
       
}

</style>
