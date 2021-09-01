<template>
  <section>
    <div class="service container">
      <div class="infos d-flex">
        <div class="inner">
          <p class="our">OUR SERVICES</p>
          <h3 class="tit ourwe">We Are Providing Digital services</h3>
        </div>
        <div class="controls d-flex align-items-end">
          <button
            class="but"
            type="button"
            data-bs-target="#carouselExampleControls"
            data-bs-slide="prev"
          >
            <span class=""><i class="fas fa-chevron-left"></i></span>
            <span class="visually-hidden"></span>
          </button>
          <button
            class="but but2"
            type="button"
            data-bs-target="#carouselExampleControls"
            data-bs-slide="next"
          >
            <span class=""><i class="fas fa-chevron-right"></i></span>
            <span class="visually-hidden"></span>
          </button>
        </div>
      </div>

      <div class="blocks col-12 d-flex">
        <div
          id="carouselExampleControls"
          class="carousel slide col-12"
          data-bs-ride="carousel"
        >
          <div class="carousel-inner">
            <div class="carousel-item active">
              <div class="genblock d-flex justify-content-between flex-wrap">
                <div
                  class="block bl1 d-flex flex-column align-items-center"
                  v-on:mouseover="changeColor"
                  v-on:mouseleave="changeView"
                >
                  <div class="imgg"><img src="img/group13.png" alt="" /></div>
                  <p class="gentit">Web Development</p>
                  <p class="sectit">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmodtempor incididunt ut labore et dolore
                  </p>
                  <div class="ent ent1">
                    <a href="#" class="white"
                      ><i class="fas fa-arrow-right"></i
                    ></a>
                  </div>
                </div>

                <div
                  class="block bl2 d-flex flex-column align-items-center"
                  v-on:mouseover="changeColor2"
                  v-on:mouseleave="changeView2"
                >
                  <div class="imgg"><img src="img/group13.png" alt="" /></div>
                  <p class="gentit">Web Development</p>
                  <p class="sectit">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmodtempor incididunt ut labore et dolore
                  </p>
                  <div class="ent ent2">
                    <a href="#" class="white"
                      ><i class="fas fa-arrow-right"></i
                    ></a>
                  </div>
                </div>
                <div
                  class="block bl3 d-flex flex-column align-items-center"
                  v-on:mouseover="changeColor3"
                  v-on:mouseleave="changeView3"
                >
                  <div class="imgg"><img src="img/group13.png" alt="" /></div>
                  <p class="gentit">Web Development</p>
                  <p class="sectit">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmodtempor incididunt ut labore et dolore
                  </p>
                  <div class="ent ent3">
                    <a href="#" class="white"
                      ><i class="fas fa-arrow-right"></i
                    ></a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import $ from "jquery";

export default {
  data() {
    return {};
  },
  methods: {
    changeColor: function () {
      $(".ent1").addClass("act");
    },
    changeView: function () {
      $(".ent1").removeClass("act");
    },
    changeColor2: function () {
      $(".ent2").addClass("act");
    },
    changeView2: function () {
      $(".ent2").removeClass("act");
    },
    changeColor3: function () {
      $(".ent3").addClass("act");
    },
    changeView3: function () {
      $(".ent3").removeClass("act");
    },
  },
};
</script>
<style>
.service {
  margin-top: 201px;
}
.our {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 30px;
  letter-spacing: 0.15em;
  color: #2370c8;
  text-align: center;
}

.ourwe {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 500;
  font-size: 48px;
  line-height: 56px;
  color: #262a4e;
  text-align: center;
  margin-bottom: 20px;
}
.blocks {
  margin-top: 69px;
  margin-bottom: 222px;
}
.block {
  width: 31%;
  height: 337px;
  background: #e5f3fe;
  border: 3px solid #cfeaff;
  box-sizing: border-box;
  transition: all 0.5s;
  position: relative;
}
.block:hover {
  background: #ffffff;
  border: 2px solid #2370c8;
  box-sizing: border-box;
  box-shadow: 0px 4px 12px #d2ebff;
  height: 316px;
}
.imgg {
  margin: 39px 0 25px;
}
.gentit {
  font-family: "Roboto";
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 23px;
  color: #262a4e;
}
.sectit {
  font-family: "Roboto";
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  text-align: center;
  color: #646464;
}

.ent {
  padding: 5px 12px;
  background: #2370c8;
  box-shadow: 0px 8px 20px rgba(35, 112, 200, 0.32);
  font-size: 20px;
  border-radius: 50%;
  color: white;
  position: absolute;
  bottom: -6%;
  display: none;
}
.act {
  display: block;
}
.white {
  color: white;
}
.controls {
  width: 119px;
  margin-left: 100px;
}
.but {
  color: rgb(139, 139, 139);
  padding: 0 15px;
  height: 40px;
  border: none;
  border-radius: 50%;
  transition: 0.5s;
}
.but:hover {
  background: #2370c8;
  box-shadow: 0px 4px 24px rgba(35, 112, 200, 0.24);
  color: white;
}
.but2 {
  margin-left: 29px;
}
.inner {
  margin-left: auto;
}
.left {
  height: 514px;
  background: #e7e7e7;
}
@media (max-width:767px) {
    h3, .tit{
        font-size: 26px;
line-height: 30px;
    }
}
</style>