<template>
<section class="moreblue">
<div class="clients container">

<h4 class="ourwe">
  We’re trusted by clients.
</h4>
<div class="aggregat d-flex flex-wrap justify-content-between">
<div class="client d-flex flex-column justify-content-between align-items-center" v-for="(obj, key) in trustJSON" :key="key">
  <div class="circle"></div>
  <p class="clname">{{obj.title}}</p>
  <p class="clprof">{{obj.txt}}</p>
  <p class="clabout">{{obj.text}}</p>
</div>
</div>

</div>
</section>
</template>
<script>
export default {
    data: () => (
        {
            trustJSON: [
                {
                img: 'img/group13.png',
                title: 'Mina Whatson',
                txt: 'CONSULTANT',
                text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which dont look even slightlybelievable. If you are going to use a passage of Lorem Ipsum, '
                },
                {
                img: 'img/group13.png',
                title: 'Mina Whatson',
                txt: 'CONSULTANT',
                text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which dont look even slightlybelievable. If you are going to use a passage of Lorem Ipsum, '
                }
            ]
        }
    )
}
</script>
<style scoped>
h4{
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 500;
    font-size: 48px;
    line-height: 56px;
    color: #FFFFFF;
    margin: auto;
    text-align: center;
}
.moreblue{
    background: rgba(55, 130, 215, 0.9);
}
.clients{
    padding: 132px 0 84px;
}
.client{
    width: 48%;
    margin-top: 44px;
    background: rgba(55, 130, 215, 0.5);
border: 1px solid #6AB0FF;
box-sizing: border-box;
padding: 52px 0 48px;
}
.circle{
    width: 68px;
height: 68px;
background: #E7E7E7;
border-radius: 50%;
}
.clname{
    font-family: 'Roboto';
font-style: normal;
font-weight: 500;
font-size: 20px;
line-height: 20px;
text-align: center;
letter-spacing: 0.01em;
color: #FFFFFF;
margin-bottom: 4px;
margin-top: 20px;
}
.clprof{
    font-family: 'Roboto';
font-style: normal;
font-weight: normal;
font-size: 16px;
text-align: center;
letter-spacing: 0.01em;
color: #FFFFFF;
}
.clabout{
font-family: 'Roboto';
font-style: normal;
font-weight: normal;
font-size: 16px;
line-height: 25px;
text-align: center;
letter-spacing: 0.01em;
color: #F2F2F2;
}
@media (max-width:767px) {
    .client{
        width: 100%;
        margin: 5px auto;
            }

}
</style>