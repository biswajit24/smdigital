<template>
  <div class="banner">
        <b-container>
            <b-row class="left-text">
                <b-col class="left_content">
                    <p class="welcome">welcome to</p>
                    <h2 class="text-capitalize text_1">the next generation of <br><span> digital</span> ocean</h2>
                    <p class="text_2">To be the best agency , by empowering businesses with the full potential of internet.
                        One day, all businesses will have the opportunity to come online to drive a
                        new era of development, growth, and productivity along with their brand name.
                    </p>
                    <b-button class="text-capitalize read">read more</b-button>
                </b-col>
                <b-col class="right_img">
                    <div class="circle"></div>
                    <img src="../static/business_img.png" class="img-1" alt="">
                    <div class="circle_2"></div>
                </b-col>
            </b-row>
        </b-container>
  </div>
</template>

<script>
export default {
    name:'Banner_vue',

}
</script>

<style scoped>
.banner {
    background: #1c233f;
    clip-path: polygon(100% 0, 100% 67%, 93% 97%, 7% 97%, 0 100%, 0% 0%);
    width: 100%;
    height: auto;
    padding: 50px 0px;
    margin-top: 45px;
}
.circle {
    width: 90px;
    height: 90px;
    background: linear-gradient(to bottom, #1c233f, #163a96);
    border-radius: 50%;
    position: absolute;
    top: 16%;
    left: 19%;
    animation: zoom-in-zoom-out 8s infinite;
}
.circle_2 {
    width: 70px;
    height: 70px;
    background: linear-gradient(to bottom, #1c233f, #163a96);
    border-radius: 50%;
    position: absolute;
    top: 16%;
    left: 82%;
    animation: zoom-in-zoom-out 5s infinite;
}
@keyframes zoom-in-zoom-out {
    0% {
        transform: scale(1, 1);
    }
    50% {
        transform: scale(1.2, 1.2);
    }
    100% {
        transform: scale(1, 1);
    }
}
.img-1 {
    position: relative;
    width: 73%;
}
h2 {
    font-size: 37px;
}
.text_1 {
    color: #fff;
    margin-bottom: 20px;
    font-weight: 700;
    letter-spacing: 2px;
}
.welcome{
    color: #fff;
    text-transform: uppercase;
    letter-spacing: 5px;
}
.text_2 {
    color: #fff;
    margin-bottom: 20px;
}
.left-text {
    align-items: center;
}
.right_img {
    display: flex;
    justify-content: flex-end;
    position: relative;
}
span {
    color: #f7bc08;
    font-weight: 800;
}
.read,
.get {
    background: transparent !important;
    border-radius: 40px !important;
    padding: 10px 20px;
    margin-right: 5px;
}

.read:hover,
.get:hover {
    background: #f7bc08 !important;
    color: #1c233f;
}

@media screen and (max-width:1140px){
    .text_1{
        font-size: 35px;
    }
}
@media screen and (max-width:992px){
    .text_1{
        font-size: 25px;
    }
    .text_2{
        font-size: 13px;
    }
    .read, .get{
        font-size: 13px;
    }
}
@media screen and (max-width:768px){
    .left-text{
        flex-direction: column;
    }
    .img-1{
        width: 60%;
    }
    .circle{
        left: 28%;
        width: 16%;
        height: 32%;
        object-fit: scale-down;
    }
    .text_1{
        font-size: 28px;
    }
}
@media screen and (max-width:600px){
    .text_2, .get,.read{
        font-size: 11px;
        line-height: 19px;
    }
}
@media screen and (max-width:480px){
    .circle_2{
        width: 12%;
        height: 24%;
    }
}
@media screen and (max-width:375px){
    .text_1{
        font-size: 22px;
    }
    .read, .get{
        padding: 7px 10px;
        font-size: 10px;
    }
}
@media screen and (max-width:320px){
     .text_1{
        font-size: 18px;
    }
    .call_num, .email {
        font-size: 15px;
    }
}
</style>