<template>
  <section>
    <div class="about container d-flex justify-content-between flex-wrap">
      <div class="left col-12 col-lg-5"></div>
      <div class="right col-12 col-lg-6">
        <p class="ourtxt">ABOUT US</p>
        <p class="tit">We design, build brands & digital projects.</p>
        <p class="abouttxt">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit
          <span class="place"
            >in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
            Excepteur sint occaecat cupidatat non proident,</span
          >
        </p>
        <a href="#" class="learn">Read More</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
    
}
</script>
<style scoped>
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
.abouttxt{
    font-family: 'Roboto';
font-style: normal;
font-weight: normal;
font-size: 16px;
line-height: 24px;
color: #646464;
}
.place{
    margin-top: 20px;
}

.about{
    margin-bottom: 270px;
}
@media (max-width:767px) {
    h3, .tit{
        font-size: 26px;
line-height: 30px;
    }
}
</style>