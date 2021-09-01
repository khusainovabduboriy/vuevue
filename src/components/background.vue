<template>
    <div class="apple">
    <img src="img/qwerty123.jpg" alt="" class="img" />
    <div class="head-info container">
    <h1 class="title">Creative
        Digital Agency</h1>
<p class="info-txt">Lorem ipsum dolor sit amet, consectetur adipiscing elit,
    sed do eiusmod tempor incididunt.</p>

<a href="#" class="learn">Learn More</a>

</div>



    </div>

</template>
<style scoped>
.img {
  position: absolute;
  z-index: -1;
  width: 100%;
  height: 100vh;
  top: 0;
  left: 0;
}
.title{
    font-family: 'Roboto';
font-size: 72px;
line-height: 85px;
color: #FFFFFF;
width: 465px;
}

.head-info{
    margin-top: 172px;
}
.info-txt{
    font-family: 'Roboto';
font-style: normal;
font-weight: normal;
font-size: 16px;
line-height: 27px;
color: #FAFAFA;
width: 443px;
margin-top: 26px;
}

.learn{
    font-family: 'Roboto';
font-style: normal;
font-weight: bold;
font-size: 16px;
line-height: 80px;
color: #FFFFFF;
padding: 19px 33px;
background: #2370C8;
border-radius: 30px;
transition: 0.5s;
}
.learn:hover{
    text-shadow: 0px 5px 10px black;
    color: white;
}
@media(max-width:767px){
        .title{
       font-size: 50px;
        line-height: 58px;
        width: 100%;
    }
      .info-txt{
        width: 100%;
    }
}
</style>