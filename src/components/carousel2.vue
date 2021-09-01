<template>
    <section class="mb container">

<div class="car2info">
    <p class="our">OUR PORTFOLIO</p>
    <p class="tit ourwe">Take A Look At Our Latest Work</p>
</div>
<div id="carouselExampleInterval" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active" data-bs-interval="10000">
        <div class="carousel2 d-flex flex-wrap justify-content-between">
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
        </div>
      </div>
      <div class="carousel-item" data-bs-interval="2000">
        <div class="carousel2 d-flex flex-wrap justify-content-between">
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
        </div>
      </div>
      <div class="carousel-item">
        <div class="carousel2 d-flex flex-wrap justify-content-between">
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
            <div class="regtangle"></div>
        </div>
      </div>
    </div>
    <div class="control2">
    <button class="but but2 butt3" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="prev">
      <span class=""><i class="fas fa-chevron-left"></i></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="but but2" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="next">
      <span class=""><i class="fas fa-chevron-right"></i></span>
      <span class="visually-hidden">Next</span>
    </button></div>
  </div>


</section>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.regtangle{
    background: #E7E7E7;
    height: 343px;
    width: 32%;
    margin-bottom: 25px;
}
.carousel2{
    margin: auto;
    margin-top: 42px;
}

.control2{
    width: max-content;
    margin: auto;
}
.mb{
    
    margin-bottom: 180px;
}
.but2{
    height: 43px;
    width: 43px;
}
.butt3{
    margin: 0;
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
@media (max-width:767px) {
    .regtangle{
width: 48%;
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