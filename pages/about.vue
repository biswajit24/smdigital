<template>
<div class="about">
    <Navbarportion />
    <h4 class="text-center text-capitalize text_heading mt-5">creative team that gets about</h4>
    <div class="line"></div>
    <div class="line_2"></div>
    <b-container>
        <b-row class="mt-5 content_align">
            <b-col class="mt-5 img_align">
                <div class="images">
                    <img src="../static/aboutpage_img1.png" class="first_img" alt="">
                </div>
                <img src="../static/aboutpage_img2.png" class="second_img" alt="">
            </b-col>
            <b-col class="mt-5">
                <strong class="text-capitalize about_us">about
                    <hr>
                </strong>
                <h3 class="text-capitalize">design & digital-solutions</h3>
                <p class="text_1">We want employees to put in long days, respond to their emails at all hours, and willingly donate their off-hours — nights, weekends, vacation — without complaining.
                </p>
                <b-row>
                    <b-col cols="1"></b-col>
                    <b-col>
                        <p class="text_3">We think strategy, UI design, and UX design</p>
                    </b-col>
                </b-row>
            </b-col>
        </b-row>
    </b-container>
    <div class="background mt-5">
      <p class="text-capitalize text_2">we are located in <span>kolkata</span></p>
    </div>

    <b-container>
        <b-row class="mt-4 content_align">
            <b-col class="mt-5">
                <strong class="text-capitalize about_company">Our solutions begin with startup
                    <hr>
                </strong>
                <p class="text_1">
                  Our team of designers and developers are perfectionists who love what they do – we thrive off pushing the boundaries of our clients’ expectations and our own capabilities.
                </p>
                <b-row>
                    <b-col>
                        <b-button class="text-capitalize get">get in touch</b-button>
                    </b-col>
                </b-row>
            </b-col>
            <b-col class="mt-5 right">
                <div class="image_right">
                    <img src="../static/aboutpage_img3.png" class="first_img_2" alt="">
                </div>
            </b-col>
        </b-row>
    </b-container>
    <Footerportion class="mt-4"/>
</div>
</template>

<script>
export default {
    name: 'About_vue',
    methods: {

    }

}
</script>

<style scoped>
*{
    font-family: 'Raleway', sans-serif;
}
.text_heading {
    position: relative;
    top: 50px;
    font-weight: 700;
}

.line {
    width: 120px;
    height: 2px;
    background: #f7bc08;
    margin: auto;
    border-radius: 10px;
    position: relative;
    top: 51px;
}

.line_2 {
    width: 40px;
    height: 5px;
    background: #1c233f;
    margin: auto;
    border-radius: 10px;
    position: relative;
    top: 47px;
}

.first_img {
    position: relative;
    border-radius: 10px;
    width: 65%;
}
.first_img_2{
   width: 75%;
}
.second_img {
    width: 38%;
    position: absolute;
    top: 35%;
    left: 50%;
    border-radius: 10px;
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    animation: zoom-in-zoom-out 8s infinite;
}

@keyframes zoom-in-zoom-out {
    0% {
        transform: scale(0.9, 0.9);
    }

    50% {
        transform: scale(1, 1);
    }

    100% {
        transform: scale(0.9, 0.9);
    }
}
.about_us{
   font-size: 20px;
   color: #1c233f; 
}
.about_company {
    font-size: 20px;
    color: #f7bc08;
}
h3{
  color: #f7bc08;
}
h4{
  color: #1c233f;
  line-height: 36px;
}
.background{
  background: url(../static/background_img.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  box-sizing: border-box;
  width: 100%;
  height: 500px;
  position: relative;
  top: 20px;
  display: grid;
  place-items: center;
  clip-path: polygon(100% 0, 100% 67%, 93% 97%, 7% 97%, 0 100%, 0% 0%);
}
.background::before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 50%;
  height: 100%;
  background: #1c233f;
  opacity: 0.6;
  transition: 0.5s;
}
.background:hover::before{
  content: '';
  width: 100%;
  height: 100%;
  background: #1c233f;
  transition: 0.5s;
}
.text_2{
  font-size: 35px;
  color: #fff;
  font-weight: 500;
  margin: 0px;
  position: relative;
  z-index: 10;
}
span{
  color: #f7bc08;
  font-size: 40px;
  font-weight: 700;
}
.text_3{
    font-size: 22px;
    color: #1c233f;
    font-weight: 500;
}
.get{
  background: #1c233f;
  border: none;
}
.get:hover{
  background: #f7bc08;
  transition: 0.5s;
  color: #1c233f;
}
.right{
  display: flex;
  justify-content: flex-end;
  width: 100%;
}
.image_right{
  text-align: right;
}

@media screen and (max-width:992px){
    h3{
        font-size: 25px;
    }
    .text_1{
        font-size: 13px;
    }
    h4{
        font-size: 21px;
    }
}
@media screen and (max-width:768px){
    .second_img{
        width: 33%;
        top: 51%;
    }
    .text_3{
        font-size: 20px;
    }
    .content_align{
        flex-direction: column;
    }
    .first_img_2{
        animation: moveTobottom 5s infinite;
    }
    @keyframes moveTobottom {
    0% {
        transform: translateY(0%);
    }
    50% {
        transform: translateY(-15%);
    }
    }
    .text_2{
        font-size: 24px;
    }
    span{
        font-size: 32px;
    }
}
@media screen and (max-width:568px){
    .about_company{
        font-size: 21px;
    }
}
@media screen and (max-width:480px){
    h3{
        font-size: 20px;
    }
    .about_company{
        font-size: 18px;
    }
    span{
        display: grid;
    }
    .text_3{
        font-size: 18px;
    }
    .first_img{
        visibility: hidden;
    }
    .img_align{
        display: flex;
        justify-content: center;
    }
    .second_img{
        width: 48%;
        top: 5%;
        left: 24%;
    }
}
@media screen and (max-width:360px){
    .text_3{
        font-size: 14px;
    }
}
@media screen and (max-width:320px){
    .text_heading{
        font-size: 18px;
    }
}
</style>