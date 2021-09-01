<template>
    <section class="lemon">
<div class="innerplace container d-flex justify-content-between flex-wrap">

<div class="cardi d-flex flex-column align-items-center" v-for="(obj, key) in lemonJSON" :key="key">
        <div class="imgg"><img src="img/group13.png" alt=""></div>  
      <p class="gentit">{{ obj.title }}</p>
      <p class="sectit"> {{ obj.txt }} </p>
</div>



</div>




</section>
</template>
<script>
export default {
    data: () => (
        {
            lemonJSON: [
                {
                img: 'img/group13.png',
                title: 'Smart planing',
                txt: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmodtempor incididunt ut labore et dolore'
                },
                {
                img: 'img/group13.png',
                title: 'Our partnership',
                txt: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmodtempor incididunt ut labore et dolore'
                },
                {
                img: 'img/group13.png',
                title: 'Super ideas',
                txt: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmodtempor incididunt ut labore et dolore'
                }
            ]
        }
    )
}
</script>

<style scoped>
.lemon{
    background: #F2F9FF;
    height: max-content;
    padding: 82px 0;
    margin-bottom: 180px;
}

.innerplace{
    border: 3px solid white;
    margin:auto;
}
.cardi{
    margin: auto;
    width: 32%;
}
@media (max-width:767px) {
    .cardi{
 width: 48%;
}
}
</style>